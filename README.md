# vscode_installaiton
cmd to install vscode in ubuntu

Step 1: Update Package List

    sudo apt-get update

Step 2: Install Dependencies

    sudo apt-get install software-properties-common apt-transport-https wget

Step 3: Import Microsoft GPG Key

    wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo gpg --dearmor -o /usr/share/keyrings/microsoft-archive-keyring.gpg

Step 4: Add VSCode Repository

    echo "deb [arch=amd64 signed-by=/usr/share/keyrings/microsoft-archive-keyring.gpg] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list > /dev/null

Step 5: Update Package List Again

    sudo apt-get update

Step 6: Install Visual Studio Code

    sudo apt-get install code

Step 7: Launch Visual Studio Code

    code
