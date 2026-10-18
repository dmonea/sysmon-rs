# SysMon-rs

**SysMon-rs** is a simple and quick System Monitor written in Rust.

This program isn't too fancy. It's just a straightforward project I made for fun. 

**No AI has been used when developing this program.**

Used libraries: `ratatui, sysino`

## How to install

### Linux

1. Download the archive from the Releases page, or from the terminal:
```zsh
curl -LO https://github.com/dmonea/sysmon-rs/releases/download/v0.1.0/sysmon-x86_64-unknown-linux-gnu.tar.gz
```
2. Unpack it. This extracts the files from the archive:
```zsh
tar xzf sysmon-x86_64-unknown-linux-gnu.tar.gz
```
3. Move it to a folder where the system looks for programs:
```zsh
sudo mv sysmon /usr/local/bin/
```
4. Run it from anywhere:
```zsh
sysmon
```

If you don't have admin rights on Linux, use `~/.local/bin` and don't use `sudo`.

If the program won't start and it displays "permission denied", run `chmod +x sysmon`.

### macOS

1. Download and unpack (Apple Silicon):
```zsh
curl -LO https://github.com/dmonea/sysmon-rs/releases/download/v0.1.0/sysmon-aarch64-apple-darwin.tar.gz
tar xzf sysmon-aarch64-apple-darwin.tar.gz
```
2. Remove the "downloaded from internet" flag from the file:
```zsh
xattr -d com.apple.quarantine sysmon
```
3. Move it onto the search path and run it:
```zsh
sudo mv sysmon /usr/local/bin
sysmon
```

If the `/usr/local/bin` doesn't exist on Apple Silicon, you can create it with:
```zsh
sudo mkdir -p /usr/local/bin
```
Or you can use `~/.local/bin` instead, but you'll have to add it to your `PATH`.

### Windows

1. Download `sysmon--x86_64-pc-windows-msvc.zip` from the Releases page.
2. Right-click on the zip and choose **Extract All**. You'll get `sysmon.exe`.
3. Run it. Open **Windows Terminal**, use `cd` to navigate to where you extracted the `.exe` file and start it:
```powershell
cd $HOME\Downloads\sysmon-x86_64-pc-windows-msvc
.\sysmon.exe
```
