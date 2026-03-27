# Run gemini-cli within termux

### This instruction is for bare-metal termux
## Instruction for proot-distro see [here](https://github.com/arfshl/termux-gemini-cli/blob/main/proot-distro.md)

1. Upgrade All Packages

       apt update && apt upgrade -y -o Dpkg::Options::="--force-confold"

2. Install nodejs and build-essential

       apt install nodejs build-essential -y

3. Install gemini-cli

       npm install -g @google/gemini-cli --ignore-scripts
   
5. Use `gemini` command for first run
6. Click number 1 to login with google
7. gemini will ask for restart
8. An login URL will be displayed, visit it with your browser
9. Login with your google account as usual
10. Copy and paste your authorization code on termux (don't share this code with anyone!)
11. Done! gemini-cli installed
