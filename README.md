# Powerful Automation Bot for the ZugChain Airdrop Ecosystem

An advanced automation bot for the ZugChain Airdrop ecosystem, featuring auto-login, daily check-ins, and verified mission completion.

---

## 📋 Table of Contents
- [Features](#-features)
- [Requirements](#-requirements)
- [Installation (Setup Guide)](#-installation-setup-guide)
- [Configuration (Settings)](#-configuration-settings)
- [How to Run](#-how-to-run)

## ✨ Features

| Feature | Description | Status |
| :--- | :--- | :--- |
| **Auto Login** | Secure wallet signature login (Metamask standard) | ✅ |
| **Time Scheduler** | Runs automatically every day at 00:00 UTC | ✅ |
| **Daily Check-In** | Automatically claims daily rewards | ✅ |
| **Faucet** | Auto-claim faucet & captcha solving | ✅ |
| **Staking** | Automatically stakes ZUG for extra points | ✅ |
| **Smart Verification** | On-chain task validation mechanism | ✅ |
| **Stealth Mode** | Realistic User-Agent rotation & behavior simulation | ✅ |
| **Multi-Account** | Unlimited multi-account support | ✅ |
| **Sipal Logging** | Clean, informative, and elegant console logs | ✅ |

## 🛠 Requirements

Before getting started, make sure you have the following installed on your system:

1. **Node.js** – Required. Download from [nodejs.org](https://nodejs.org/) and choose the **LTS version (v18 or newer)**.
2. **Git** – Required. Download from [git-scm.com](https://git-scm.com/downloads).
3. **2Captcha API Key** – Required to solve faucet captchas (must have balance).

## 📦 Installation (Setup Guide)

Follow these steps carefully, suitable for beginners:

### 1. Download the Bot
Open your terminal (Command Prompt or PowerShell) and run:

```bash
git https://github.com/TestnetMaster29/zugchain-autoBot
cd zugchain-autoBot
```

### 2. Install Dependencies
In the same terminal, install all required packages:

```bash
npm install
```

*Wait until the installation completes. This may take a few minutes.*

## ⚙️ Configuration (Settings)

### 1. Create the Account File (`accounts.json`)
You need to create a file to store your account data:

1. Locate the file named `accounts_tmp.json` in the bot folder.
2. Rename it to `accounts.json`.
3. Open the file using Notepad or any text editor.
4. Fill in your account details following this format:

```json
{
  "twoCaptchaApiKey": "YOUR_2CAPTCHA_API_KEY",
  "accounts": [
    {
      "name": "Account 1",
      "privateKey": "YOUR_METAMASK_PRIVATE_KEY",
      "proxy": "http://user:pass@ip:port"
    }
  ]
}
```

> **Notes:**
> - `privateKey`: Your evm wallet private key (**keep it secret!**).
> - `proxy`: Optional. Leave empty if you are not using a proxy.
> - `twoCaptchaApiKey`: Required to bypass captcha during faucet claims.

### 2. General Configuration (`config.json`)
The `config.json` file is preconfigured by default.

You do **not** need to change anything unless instructed by a SipalDrop update.

## 🚀 How to Run

Once everything is set up, start the bot by running:

```bash
npm start
```

ENJOY !!!!
