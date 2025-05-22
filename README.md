# Linux-VM
- Hosted a Linux Virtual Machine on my PC to teach myself Linux Terminal Prompts using Ubuntu distro
- Configured MSI motherboard to allocate computing resources and storage to co-host VM VirtualBox software


## What I Did

- Created a Virtual Machine using **VirtualBox** and installed the **Ubuntu** distribution.
- Allocated system resources (CPU, RAM, disk) through my **MSI motherboard BIOS** to ensure smooth VM performance.
- Practiced core **Linux terminal commands** to build familiarity with bash scripting and system navigation.
- Installed essential tools like `git`, `curl`, `vim`, and `build-essential` using `apt`.
- Took screenshots to document progress and system setup.

## Commands I Practiced

```bash
sudo apt update
sudo apt install git curl vim build-essential
neofetch
curl https://example.com
```

## Additional Customizations & Installs

- Changed the Ubuntu desktop **background** to personalize the VM.
- Installed **Google Chrome** by downloading and installing the `.deb` package via terminal.
- ⛏Installed **Minecraft Java Edition** on Ubuntu using `openjdk` and the official Minecraft launcher.

### Commands Used

```bash
# Download & install Chrome
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo apt install ./google-chrome-stable_current_amd64.deb
```

# Install Java and Minecraft launcher
sudo apt install openjdk-17-jre
wget https://launcher.mojang.com/download/Minecraft.deb
sudo apt install ./Minecraft.deb

## Docker & Containerization

To take this project a step further, I installed Docker inside the Linux VM and successfully launched my first containerized web server.

### 🔧 What I Did:
- Installed Docker using `apt`
- Ran the official **Nginx** image in a container mapped to `localhost:8080`
- Verified that the container served a live web page from within the VM

### Commands Used:
```bash
sudo apt install docker.io
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
# (after logout/login or newgrp docker)
docker run hello-world
docker run -d -p 8080:80 nginx
```
