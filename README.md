# SysMon-rs

**SysMon-rs** is a simple and quick System Monitor written in Rust.

This program isn't too fancy. It's just a straightforward project I made for fun. 

**No AI has been used when developing this program.**

Used libraries: `ratatui, sysino`

## How to install

### Linux

1. Download the release archive file corresponding to your system
2. Unzip it
3. Move it to a folder where the system looks for programs: `sudo mv sysmon-rs /usr/local/bin/sysmon`
4. Run it from anywhere: `sysmon` (use `sysmon-rs` if you haven't renamed it to "sysmon")

If you don't have admin rights on Linux, use `~/.local/bin` and don't use `sudo`.

If the program won't start and it displays "permission denied", run `chmod +x sysmon`.

### macOS

1. Download and unpack (Apple Silicon):
2. Remove the "downloade from internet" flag from the file:
```zsh
xattr -d com.apple.quarantine sysmon
```
3. Move it onto the search path and run it:
```
sudo mv sysmon /usr/local/bin
sysmon
```
