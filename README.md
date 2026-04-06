# 🤖 Auto Scripts — MT5 Script Manager

<div align="center">

![Platform](https://img.shields.io/badge/Platform-MetaTrader%205-blue?style=for-the-badge&logo=windows)
![Language](https://img.shields.io/badge/Language-C%23%20%2F%20WinForms-purple?style=for-the-badge&logo=dotnet)
![Version](https://img.shields.io/badge/Version-1.0.0-gold?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**A professional desktop application for managing and running MT5 trading scripts with a modern dark UI.**

</div>

---

## 📸 UI Preview

> Dark-themed, borderless WinForms application with sidebar navigation, live MT5 connection status, script runner, and order preview grid.

| Component | Description |
|-----------|-------------|
| 🎨 Theme | Dark Navy (`#12_1428`) with Blue/Red/Gold accents |
| 🖥️ Framework | .NET WinForms (C#) |
| 📐 Window | 1300 × 920 px, resizable, borderless, draggable |

---

## ✨ Features

- **Close All Orders Script** — closes all open positions and cancels all pending orders on the MT5 account instantly
- **Live MT5 Connection Panel** — shows server, login, and connection status with one-click disconnect/reconnect
- **Order Preview** — view open positions and pending orders in grid tables before executing
- **Confirmation Gate** — requires checkbox confirmation before running any destructive script
- **Animated Progress Bar** — step-by-step visual feedback during script execution
- **Status Bar** — real-time clock and live script status messages
- **Modern Borderless Window** — custom title bar with minimize, maximize, and close controls

---

## 🗂️ Script Library

| Script Name | Type | Description |
|-------------|------|-------------|
| ❌ Close All Orders | Utility | Closes all open positions & pending orders |
| *(more scripts coming soon)* | — | — |

---

## 🖥️ UI Structure

```
┌─────────────────────────────────────────────────────┐
│  Top Bar  [Auto Scripts — MT5 Script Manager]  [─□✕] │
├──────────┬──────────────────────────────────────────┤
│          │  Header Card  [Script Name + Run Button]  │
│ Sidebar  ├──────────────────────────────────────────┤
│          │  Script Info Card  |  What It Does Card   │
│ 🗂 Library│  ─────────────────────────────────────── │
│ 🏠 Home  │  Preview Card                             │
│ 📊 Dash  │    ┌─ Open Positions ─┬─ Pending Orders ─┐│
│ 📅 Events│    │  EURUSD  Buy ... │  GBPUSD  Limit.. ││
│ ℹ  About │    └──────────────────┴──────────────────┘│
│ ✉  Contact│  ─────────────────────────────────────── │
│          │  Warning + Confirmation + Run Button       │
│ MT5 Conn.│                                            │
└──────────┴──────────────────────────────────────────┘
│  Status Bar               HH:MM:SS  DD.MM.YYYY       │
└─────────────────────────────────────────────────────┘
```

---

## 🎨 Color Palette

| Name | Hex | Usage |
|------|-----|-------|
| `BgDark` | `#121428` | Main background |
| `BgPanel` | `#191C37` | Sidebar |
| `BgCard` | `#1E223E` | Cards |
| `AccentBlue` | `#3F51B5` | Active nav, badges |
| `AccentRed` | `#E53935` | Run button, warnings |
| `AccentGold` | `#FB8C00` | Pending order badges |
| `AccentGreen` | `#2EA043` | Success states |
| `TextMain` | `#E6E8FF` | Primary text |
| `TextSub` | `#8C94C8` | Secondary text |

---

## ⚙️ Requirements

- [.NET 6+ / .NET Framework 4.8](https://dotnet.microsoft.com/)
- Windows OS (WinForms)
- MetaTrader 5 terminal (for live trading)
- Visual Studio 2022+ (recommended)

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/your-username/auto-scripts-mt5.git

# 2. Open in Visual Studio
# Open WinFormsApp1.sln

# 3. Build & Run
# Press F5 or use Build > Start Debugging
```

---

## 📋 How to Use — Close All Orders Script

1. Launch the application
2. Verify MT5 connection status in the bottom-left sidebar (green dot = connected)
3. Review **Open Positions** and **Pending Orders** in the Preview section
4. Check the confirmation box: *"I understand that this will close all positions..."*
5. Click **▶ Run Script**
6. Watch the progress bar and status bar for real-time feedback
7. All orders will be marked as **Closed / Cancelled** upon completion

> ⚠️ **Warning:** This action is irreversible. All open positions and pending orders will be permanently closed/canceled.

---

## 📁 Project Structure

```
WinFormsApp1/
├── Form1.cs              # Main form — all UI and logic
├── Form1.Designer.cs     # Auto-generated designer file
├── Program.cs            # Entry point
└── WinFormsApp1.csproj   # Project file
```

---

## 🛠️ Built With

- **C# / WinForms** — UI framework
- **System.Drawing** — Custom painting & GDI+
- **System.Windows.Forms.Timer** — Script progress animation
- **DataGridView** — Order tables with custom cell formatting

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">
Made with ❤️ by <strong>Auto Scripts Team</strong> — v1.0.0
</div>
