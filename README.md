# Kali-Linux-Setup
personal commands list to run after install Kali Linux for my main computer

## Upgrade System
```bash
sudo apt update
sudo apt upgrade -y
```

## Install Nvidia Drivers

Install the nvidia driver, neglect the conflict warning

```
apt-get install nvidia-driver -y
```

Remove the open source driver

```
sudo nano /etc/modprobe.d/blacklist-nouveau.conf
```


```
blacklist nouveau
options nouveau modeset=0
alias nouveau off
```

save file and exit

```bash
update-initramfs -u
```

```bash
reboot
```

## Install Main Apps

Install Main Tools
```bash
sudo apt install curl wget apt-transport-https -y
```


[Brave Browser](https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/brave-browser.sh) :

```bash
wget "https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/brave-browser.sh" && chmod +x ./brave-browser.sh && ./brave-browser.sh
```

[Github Desktop](https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/github-desktop.sh) :

```bash
wget "https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/github-desktop.sh" && chmod +x ./github-desktop.sh && ./github-desktop.sh
```

[Discord](https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/discord.sh):

```bash
wget "https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/discord.sh" && chmod +x ./discord.sh && ./discord.sh
```

[Better Discord](https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/better-discord.sh):

```bash
wget "https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/better-discord.sh" && chmod +x ./better-discord.sh && ./better-discord.sh
```

[Discord](https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/vscode.sh):

```bash
wget "https://raw.githubusercontent.com/hirusha-adi/Kali-Linux-Setup/main/scripts/vscode.sh" && chmod +x ./vscode.sh && ./vscode.sh
```
