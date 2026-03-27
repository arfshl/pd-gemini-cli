# Run gemini-cli within proot-distro

### This instruction is for debian/ubuntu based distros

1. Install nodejs 24.x

       apt update && apt install curl -y && apt-get install -y curl && curl -L -o setupnode https://deb.nodesource.com/setup_24.x && chmod +x setupnode && ./setupnode && apt install nodejs -y 

2. Install yarn

       npm install -g yarn

3. Install gemini-cli

       yarn global add @google/gemini-cli

4. Use `gemini` command for first run
5. Click number 1 to login with google
6. gemini will ask for restart
7. An login URL will be displayed, visit it with your browser
8. Login with your google account as usual
9. Copy and paste your authorization code on termux (don't share this code with anyone!)
10. Done! gemini-cli installed

### Debian stable proot-distro rootfs with gemini-cli (Containerized) (ARM64)
Useful if you want to use gemini-cli separated from your main termux setup or your other proot-distro rootfs

1. Install
proot-distro alias: gemini-cli-debian

       apt install proot-distro -y && PD_OVERRIDE_TARBALL_URL="https://github.com/arfshl/termux-gemini-cli/releases/download/latest/gemini-cli-debian-stable.tar.xz" PD_OVERRIDE_TARBALL_SHA256="" proot-distro install debian --override-alias gemini-cli-debian
