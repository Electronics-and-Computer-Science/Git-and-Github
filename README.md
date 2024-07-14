# Git and GitHub Installation

## Code Editor (VS Code) Installation

### Step 1
1. Download the Visual Studio Code installer for Windows. Use this [link](https://code.visualstudio.com/docs/setup/windows).

### Step 2
Once it is downloaded, run the installer (`VSCodeUserSetup-{version}.exe`). This will only take a minute.

### Step 3
By default, VS Code is installed under:
```
C:\Users\{Username}\AppData\Local\Programs\Microsoft VS Code
```

## Git Installation

### Git for Windows

#### Step 1
To download the Git installer, visit the Git's official site and go to the download page. The link for the download page is [https://git-scm.com/downloads](https://git-scm.com/downloads).

#### Step 2
Click on the downloaded installer file and select yes to continue. After selecting yes, the installation begins.

#### Step 3
Default components are automatically selected. You can also choose your required components.

#### Step 4
The default Git command-line options are selected automatically. You can choose your preferred choice. Click next to continue.

#### Step 5
The default transport backend options are selected. Click next to continue.

#### Step 6
Select your required line ending option and click next to continue.

#### Step 7
Select preferred terminal emulator and click next to continue.

#### Step 8
This is the last step that provides some extra features like system caching, credential management, and symbolic link. Select the required features and click next.

#### Step 9
The files are being extracted in this step.

### Git for Linux (Ubuntu)

#### Step 1: Start the General OS and Package Update
Run the following command:
```sh
sudo apt-get update
```

#### Step 2: Install Git
To install Git, run the following command:
```sh
sudo apt-get install git-core
```
You may be asked to confirm the download and installation.

#### Step 3: Confirm Git Installation
To confirm the installation, press the 'y' key when prompted. Once installed, verify the installation by running:
```sh
sudo git --version
```

#### Step 4: Configure Git
To configure Git for the first use:
```sh
sudo git config --global user.name "Your Name"
sudo git config --global user.email "your.email@example.com"
```

### Git for macOS

#### Step 1: Install Homebrew
Open Terminal and paste the following command:
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Step 2: Add Homebrew to Your PATH
Run the following commands:
```sh
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/$(whoami)/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

Verify Homebrew installation:
```sh
brew help
```

#### Step 3: Install Git Using Homebrew
Install Git:
```sh
brew install git
```

Verify Git installation:
```sh
git --version
```

#### Step 4: Configure Git
Set your username:
```sh
git config --global user.name "Your Name"
```

Set your email:
```sh
git config --global user.email "your.email@example.com"
```

Set your default text editor:
```sh
git config --global core.editor "code --wait"
```

Set the default branch name:
```sh
git config --global init.defaultBranch main
```

Enable colored output:
```sh
git config --global color.ui true
```

## Sign Up or Sign In to GitHub

### Step 1: Creating an Account
To sign up for an account on GitHub.com, navigate to [https://github.com/](https://github.com/) and follow the prompts.

### Step 2: Configuring Two-Factor Authentication
1. Download a TOTP app of your choice to your phone or desktop.
2. In the upper-right corner of any page on GitHub, click your profile photo, then click **Settings**.
3. In the "Access" section of the sidebar, click **Password and authentication**.
4. In the "Two-factor authentication" section of the page, click **Enable two-factor authentication**.
5. Under "Scan the QR code", do one of the following:
   - Scan the QR code with your mobile device's app. After scanning, the app displays a six-digit code that you can enter on GitHub.
   - If you can't scan the QR code, click the setup key to see a code, the TOTP secret, that you can manually enter in your TOTP app.
6. The TOTP application saves your account on GitHub and generates a new authentication code every few seconds. On GitHub, type the code into the field under "Verify the code from the app".
7. Under "Save your recovery codes", click **Download** to download your recovery codes to your device. Save them to a secure location.
8. After saving your two-factor recovery codes, click **I have saved my recovery codes** to enable two-factor authentication for your account.
9. Optionally, you can configure additional 2FA methods to reduce your risk of account lockout. For more details, see [GitHub's documentation](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication).
