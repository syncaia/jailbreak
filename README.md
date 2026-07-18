<div align="center">
  <h1 align="center">Kindle Jailbreak (Adbreak) A2Z Guide</h1>
  <p align="center">
    A complete, step-by-step documentation to jailbreak your Kindle using the new 'Adbreak' method.
  </p>
  <p align="center">
    <a href="https://github.com/rokibul/kindle-jailbreak/blob/main/LICENSE"><img src="https://img.shields.io/github/license/rokibul/kindle-jailbreak?style=flat-square" alt="License"></a>
    <a href="https://github.com/rokibul/kindle-jailbreak/releases"><img src="https://img.shields.io/github/v/release/rokibul/kindle-jailbreak?style=flat-square" alt="Version"></a>
    <img src="https://img.shields.io/badge/platform-Kindle-blue?style=flat-square" alt="Platform">
    <a href="https://github.com/rokibul/kindle-jailbreak/issues"><img src="https://img.shields.io/github/issues/rokibul/kindle-jailbreak?style=flat-square" alt="Open Issues"></a>
  </p>
</div>

[🌍 Read in English](README.md) | [📖 বাংলায় পড়ুন](README_BN.md)

---

> [!CAUTION]
> **Disclaimer:** This process will likely void your Kindle's warranty. These instructions are provided for educational purposes only. Follow any steps at your own risk. Amazon can patch this method at any time, so always check the linked written guide before starting.

## 📑 Table of Contents

- [Why Jailbreak your Kindle?](#why-jailbreak-your-kindle)
- [Phase 1: Prerequisites](#phase-1-prerequisites)
- [Phase 2: Pre-Installation (Prevent Auto-Update)](#phase-2-pre-installation-prevent-auto-update)
- [Phase 3: Exploit Execution](#phase-3-exploit-execution)
- [Phase 4: Post-Installation (Hotfix & Apps)](#phase-4-post-installation-hotfix--apps)
- [Troubleshooting & FAQ](#troubleshooting--faq)
- [Repository Structure](#repository-structure)

---

## Why Jailbreak your Kindle?

Jailbreaking can completely transform your Kindle experience. It allows you to:
- Use custom readers (like KOReader).
- Set custom lock screens.
- Remove advertisements.
- Add extra audio support.
- Access a new App Store (KindleForge).
- Run a full Linux desktop environment.

Essentially, it completely unlinks you from Amazon's ecosystem and gives you full control over your device.

---

## Phase 1: Prerequisites

Before starting, ensure your device is suitable for this jailbreak.

> [!WARNING]
> **Check Firmware:** This 'Adbreak' jailbreak works on specific firmware versions. Check the official written guide linked below to ensure your current firmware is compatible before attempting anything.

**Required Resources:**
- **Main Written Guide (Required):** [kindlemodding.org](https://kindlemodding.org)
- **Filler Files:** [Download Here](https://github.com/rokibul/kindle-jailbreak/tree/main/Kindle-Filler-Disk/MTP)
- **Update Blocker (Renameotabin):** [Download Here](https://github.com/rokibul/kindle-jailbreak/raw/refs/heads/main/mobileread-KUAL/renameotabin.zip)
- **KindleForge App Store:** [Download v4.1.0](https://github.com/rokibul/kindle-jailbreak/releases/tag/v4.1.0)
  - *If you are new to GitHub, just click on `kindleforge.zip` to download. After downloading, drag & drop the files into your Kindle's `documents` folder.*
- **Project Title for KOReader:** [Download Here](https://github.com/rokibul/kindle-jailbreak/tree/main/ProjectTitle) (Use this if you like the custom setup shown in the video).

**Mac Users Note:** You will need this command later on:
`find . -name 'details.html' -exec cp adbreak.html {} \;`
*(If it fails, use: `find ./.assets -name 'details.html' -exec cp adbreak.html {} \;`)*

---

## Phase 2: Pre-Installation (Prevent Auto-Update)

If you connect to Wi-Fi, your Kindle might automatically update and render this jailbreak useless. To prevent this, we must fill the device storage.

1. Plug your Kindle into a computer using a data cable (not just a charging cable).
2. *(Mac Users)* If the device doesn't appear, use Amazon's "Send to Kindle" app and open its "USB File Manager".
3. Download the "Filler Files" zip corresponding to your Kindle's storage size (e.g., 16GB).
4. Unzip the file. You will see many random data files.
5. Drag and drop these files into the root directory of your Kindle until the storage is almost completely full (leave about 100MB free).
6. **Important:** If there is a file named `update.bin` in the root of your Kindle, delete it immediately.
7. Unplug the Kindle from the computer. Your device will now show that it has no free space.
8. It is now safe to turn on Wi-Fi and log into your Amazon account. Any attempt to update will fail due to lack of storage.

---

## Phase 3: Exploit Execution

This jailbreak exploits a vulnerability in the Kindle's advertisement system.

### Step 1: Enable Ads
1. **If you have an Ad-supported Kindle:** You are ready to proceed.
2. **If you have an Ad-free Kindle:**
   - Log into your Amazon account and go to the "Devices" tab.
   - Select your Kindle and click "Sign up for offers".
3. **If your country doesn't support Ads:**
   - You must register your Kindle with a US Amazon account.
   - Use any US address (e.g., the White House address).
   - Use a fake US credit card generator ensuring the billing and home addresses match.
4. Wait a few minutes (about 5 mins) until ads start appearing on your Kindle's lock screen.
5. > [!IMPORTANT]
   > Once you see an ad, **IMMEDIATELY turn on Airplane Mode.**

### Step 2: Execute Exploit
1. Plug your Kindle back into the computer.
2. Look for a folder named `assets` inside the `system` folder. This is where ads are stored.
3. This folder is usually hidden:
   - **Mac:** Press `Command + Shift + .` to see hidden folders.
   - **Windows:** Go to the "View" tab in File Explorer and check "Hidden items".
4. Copy the entire `assets` folder from your Kindle to your computer.
5. Download the jailbreak files from `kindlemodding.org`.
6. Unzip the files and place them inside the `assets` folder you just copied to your computer.
7. **Run the Script:**
   - **Windows:** Double-click the `.bat` file inside the folder.
   - **Mac:** Open Terminal inside the `assets` folder (View > Show Path Bar > Right-click > "Open in Terminal"). Paste the Mac command: `find . -name 'details.html' -exec cp adbreak.html {} \;` and press Enter.
8. Now, delete the *old* `assets` folder from your Kindle device.
9. Drag the *modified new* `assets` folder from your computer into your Kindle.
10. Unplug the Kindle. It should still be in Airplane Mode.
11. Wake the device from sleep. It will try to load an ad, and the screen may act weird (turning white or disappearing).
12. **Congratulations!** The jailbreak is successfully installed.

---

## Phase 4: Post-Installation (Hotfix & Apps)

Follow these steps to make the jailbreak permanent and install apps.

### Step 1: Install Hotfix
This ensures your jailbreak survives future system updates.

1. Download the "Hotfix" (`.bin` file) from the Kindle Modding Wiki.
2. Connect the Kindle to your computer and drag the Hotfix file to the root of your Kindle.
3. Unplug the Kindle.
4. On your Kindle, go to: **Settings > Device Info > "Update Your Kindle"**. (Don't worry, it's just loading the hotfix).
5. The screen will show some text, and the device will reboot.
6. After rebooting, you will see a new book in your library called "Run Hotfix". If your device ever updates, simply running this book will restore the jailbreak.

### Step 2: Remove Filler Files
1. Ensure your Kindle is in **Airplane Mode**.
2. Since we are safe from updates, connect to your PC and delete those large filler files.
3. *Important:* Make sure to empty your computer's Recycling Bin to free up the space completely.

### Step 3: Install MRPI and KUAL
- **MRPI (MobileRead Package Installer):** Allows installing custom apps.
- **KUAL (Kindle Unified Application Launcher):** The menu to open those apps.

1. Download MRPI and KUAL (coplate version) from the Wiki.
2. Unzip the KUAL installer. Drag the two folders inside (`extensions` and `mrpackages`) to the root of your Kindle.
3. Place the MRPI `.bin` file inside the `mrpackages` folder.

### Step 4: Permanently Block Updates
1. Download the "Block Updates Package" (`renameotabin.zip`) linked in Prerequisites.
2. Unzip it and place the entire folder inside your Kindle's `extensions` folder.
3. Unplug the Kindle.
4. Go to the Kindle's search bar, type exactly `;log koal` and press Enter.
5. The screen will flash, and a new book named "KUAL" will appear in your library.
6. Open "KUAL". This is your jailbreak app launcher.
7. Inside, you will see the "Block Updates" extension. Tap it (or tap "rename" to run it).
8. The device will reboot one last time.
9. **Success!** Updates are permanently disabled. You can safely turn off Airplane Mode.

---

## Troubleshooting & FAQ

> [!NOTE]
> Here are common issues users face and how to resolve them.

**Q: My Kindle accidentally connected to Wi-Fi and updated!**
**A:** If you installed the Hotfix before this happened, you are safe! Just open the "Run Hotfix" book in your library. If you did not install the hotfix yet, your jailbreak is gone, and you may need to wait for a new exploit if Amazon patched it.

**Q: The Mac terminal script isn't working for me.**
**A:** Sometimes the structure differs slightly. Try running `find ./.assets -name 'details.html' -exec cp adbreak.html {} \;` instead of the original command.

**Q: I don't see the `update.bin` file.**
**A:** That is perfectly normal. If it's not there, just proceed to the next step.

**Q: KUAL isn't showing up in my library.**
**A:** Ensure you copied the `extensions` and `mrpackages` folders exactly to the *root* directory, not inside any other folder. Then, make sure you typed `;log koal` correctly in the search bar.

---

## Recommended Apps & Tweaks (Next Steps)

Your Kindle is now free. Here are some highly recommended apps:

1. **KindleForge (App Store):** A user-friendly app store for Kindle. Install the "Disable Ads" script from here first!
2. **HotfixUpdater:** A simple on-device tool to automate checking, downloading, and running the latest Universal Hotfix without a PC.
3. **KOReader:** Replaces the default reading interface. Supports EPUB, custom themes, custom lock screens, and better battery life.
4. **Socks Media Player:** Play music or audiobooks via Bluetooth speakers.
5. **KWordle:** Play Wordle on Kindle.
6. **Kinki:** Powerful flashcard app for learning.
7. **Gambit (K2):** Game Boy and Game Boy Color emulator.

### Awesome Kindle & Official Repository

For a complete curated list of tweaks, check out [Awesome Kindle](https://github.com/KindleTweaks/Awesome-Kindle).
Additionally, explore the [KindleForge Official Repository](https://github.com/KindleTweaks/Repository) for the complete collection of packages you can download directly to your device via KindleForge (including PEKI, Gargoyle, GNOME Games, KNotes, and more).

Here is a glimpse of what you can find:
- **Quality of Life:** HotfixUpdater, Toggle ADs, UpdateBlock Status.
- **Productivity:** Textadept, KAnki, RAnki, KPomo, Kreate, KNotes.
- **Games:** Gambit (K2), Gargoyle, GNOME Games, KShips, KWordle, KindleCraft.
- **System & Dev:** PEKI (Penguins' Epic KUAL Installer - a better looking launcher for KUAL), kTerm, Alpine Linux.
- **Audio:** LARK Player, KinAMP, SOX.

[![Watch the video](https://github.com/rokibul/kindle-jailbreak/blob/main/6sigPg.gif?raw=true)](https://www.youtube.com/watch?v=kDp3DMQsx-I "Play on YouTube")

---

## Credits
Special thanks to the following repositories and their developers for their awesome tools:
* **[HotfixUpdater](https://github.com/KindleTweaks/HotfixUpdater):** A fantastic tool for on-device hotfix updates.
* **[KindleForge](https://github.com/KindleTweaks/KindleForge):** A graphical app store for Kindle.
* **[Awesome-Kindle](https://github.com/KindleTweaks/Awesome-Kindle):** An amazing curated list of Kindle tweaks.
* **[KindleForge Repository](https://github.com/KindleTweaks/Repository):** The official repository for KindleForge packages.
* **[PEKI](https://github.com/KindleTweaks/PEKI):** An epic KUAL installer and launcher.

---

## Repository Structure

Links to important folders and files in this repository:

* 📁 [KindleForge/](./KindleForge/) - GUI Appstore for Kindle devices.
* 📁 [Kindle-Filler-Disk/](./Kindle-Filler-Disk/) - Utility to fill Kindle storage to prevent auto-updates.
* 📁 [ProjectTitle/](./ProjectTitle/) - A new view based on Cover Browser for KOReader.
* 📁 [mobileread-KUAL/](./mobileread-KUAL/) - Kindle update block package and KUAL resources.
* 🖼️ [6sigPg.gif](./6sigPg.gif) - Animated GIF used for the video tutorial.
