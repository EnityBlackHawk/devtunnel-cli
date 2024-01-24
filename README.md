# devtunnel-cli
This is a patched Microsoft's devtunnel installer script to works with Arch's repository manager (Pacman).

Miscrosoft's original script: [Link](https://tunnelsassetsdev.blob.core.windows.net/cli/install-cli.sh)

### Install:
```
sudo pacman -S devtunnel-cli-git
```

### Remove:
```
sudo pacman -R devtunnel-cli-git
sudo rm /usr/local/bin/devtunnel
```