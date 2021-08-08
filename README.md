# gpp_decrypt
gpp_decrypt is a library for decrypting cpasswords in Group Policy Preference files. You'll find this useful for a certain [hackthebox](https://hackthebox.eu) machine as well. If you're looking for the standalone binary version, see [gpp-decrypt](https://github.com/RIckConsole/gpp-decrypt)

## Usage
```rust
extern crate gpp_decrypt;

fn main() {
    let enc = "YOUR_CPASSWORD_HERE".to_string();
    let result = gpp_decrypt::gpp_decrypt(enc);
    println!("{}", result);
}
```

