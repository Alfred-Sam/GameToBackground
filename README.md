# 🎮 Game To Background

> Seamlessly convert any active game, video, or application into your live Windows desktop background when idle — and restore it with a single click!
>
> **Created by Zlac — We Love Gembull ❤️**

---

## 📖 Overview

**Game To Background** is a lightweight Windows utility that monitors your system idle time. When you step away from your PC or stop interacting for a set duration, the active foreground application (such as Google Chrome, YouTube, Twitch streams, singleplayer/idle games, or media players) is smoothly transferred behind your desktop icons into the Windows `WorkerW` wallpaper layer.

---

## ⚙️ How It Works

### 1. ⏱️ Automatic Idle Detection

- Configure your desired idle threshold (default: **30 seconds**).
- If no keyboard or mouse movement is detected for that duration, the active window is automatically resized and sent to the desktop wallpaper background.

### 2. 🖥️ Multitask Freely While in Background

- While your game or video is running as the desktop wallpaper, you can press the **`Windows Key`**, search and open **Microsoft Word**, **Steam**, **Calculator**, **Discord**, or any other software.
- You can work, type, and interact with other apps on top of the screen **without interrupting the background application**.

### 3. 🖱️ Smart Click-to-Restore

- When you are ready to resume, simply **left-click on any empty area of the desktop background**.
- The application immediately restores to its original windowed size, pops back to the foreground, and refreshes the wallpaper.

### 4. 🛡️ Anti-Cheat Safe Mode

- Automatically protects and excludes competitive games equipped with strict anti-cheat systems, such as **Counter-Strike 2 / CS:GO**, **VALORANT / Riot Vanguard**, **Apex Legends**, **Fortnite**, **Rainbow Six Siege**, **Overwatch**, **League of Legends**, and others.
- Helps prevent potential anti-cheat conflicts, game crashes, and DirectX graphics engine issues.

> **Note:** Anti-Cheat Protection is designed to reduce compatibility issues with supported games. It does not guarantee protection against every anti-cheat system or prevent all possible game-related issues.

---

## 🚀 How to Use

1. Launch `GameToBackgroundGUI.exe`.
2. Set your desired **Idle Threshold** in seconds.
3. Keep **Anti-Cheat Protection** checked (recommended).
4. Click **Start Service**.
5. Leave your favorite game, stream, or browser open.
6. Once you go idle for the configured duration, the application will automatically become your live desktop background.

---

## 🔨 Building & Publishing Standalone Executable

To compile a standalone `.exe` that runs on Windows 10/11 64-bit machines without requiring .NET to be installed, run:

```powershell
dotnet publish GameToBackgroundGUI\GameToBackgroundGUI.csproj -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true -p:EnableCompressionInSingleFile=true
```

The compiled standalone executable will be located at:

```text
GameToBackgroundGUI\bin\Release\net8.0-windows\win-x64\publish\GameToBackgroundGUI.exe
```

---

## 💻 Requirements

- **Operating System:** Windows 10 / Windows 11 (64-bit)
- **Architecture:** x64

---

## 👨‍💻 Credits & License

- **Developer:** Created by **Zlac**
- **Special Note:** *We Love Gembull* ❤️
- Distributed under the [MIT License](LICENSE).
