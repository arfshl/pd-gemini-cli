# Run gemini-cli within proot-distro

1. Install nodejs, and npm (for this example i use apt, which is for debian/ubuntu based distro)

       apt install nodejs npm -y

2. Install yarn

       npm install -g yarn

3. Install gemini-cli

       yarn global add @google/gemini-cli

4. Click number 1 to login with google
5. An login URL will be displayed, visit it with your browser
6. Login with your google account as usual
7. Copy and paste your authorization code on termux (don't share this code with anyone!)
8. Done! gemini-cli installed
