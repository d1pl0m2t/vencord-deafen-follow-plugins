# Private Plugins for Vencord

This repository contains private plugins for **Vencord**, which add new features to Discord.

### Plugins:

1. **Listen with mic muted and speak with mic off**: This plugin allows you to listen to other users even when your microphone is muted and speak without activating your mic.
2. **Follow user across voice channels**: This plugin allows you to finely follow a user as they move between voice channels.

---

## Installation

### **1. Requirements**

- **Windows / Linux**
- **Discord** or **Discord Canary** — must be installed for patching.
- Installed **Git**, **Node.js**, and **pnpm**.

### **2. Installation on Windows**

1. **Download and install Git**:  
   [https://git-scm.com/](https://git-scm.com/)
   
2. **Install Node.js**:  
   [https://nodejs.org](https://nodejs.org)

3. **Install pnpm via PowerShell (run as Administrator):**
   ```powershell
   Invoke-WebRequest https://get.pnpm.io/install.ps1 -UseBasicParsing | Invoke-Expression

4. **Clone the Vencord repository:**
   ```Open PowerShell and execute the following:
   cd Desktop
   git clone https://github.com/Vendicated/Vencord
   cd Vencord
5. **Install Dependencies:**
   ```
   pnpm install --frozen-lockfile
6. **Build the project:**
   ```
   pnpm build
7. **Apply the patch (patch Discord):**
   ```
   pnpm inject
  ## 3. Installation on Linux

 1. **Install Node.js and npm:**
  ```
  sudo apt install nodejs npm
  ```

 2. **Install pnpm:**
  ```
  npm install pnpm
  ```

 3. **Or use the alternative method:**
  ```
  curl -fsSL https://get.pnpm.io/install.sh | sh -
  ```

 4. **Clone the Vencord repository:**
  ```
  git clone https://github.com/Vendicated/Vencord
  cd Vencord
  ```

 5. **Install dependencies:**
  ```
  pnpm install --frozen-lockfile
  ```

 6. **Build the project:**
  ```
  pnpm build
  ```

 7. **Apply the patch (patch Discord):**
  ```
  sudo pnpm inject
  ```

## WARNING!!
**Before running the pnpm inject command, create a directory at the path /Vencord/src/ named userplugins and move the downloaded Follow folder and the fakeVoiceOption.ts file into it.**

  ### 4. Important Notes

   ***Before using the plugins, make sure you have Discord or Discord Canary installed. These are required for the patching process.***

   ***Download Discord:*** https://discord.com/download

   ***Download Discord Canary:*** https://discord.com/download
