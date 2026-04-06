<div align="center">

# Position Sizer MT5 / MT4

**Professional risk management and position sizing tool for MetaTrader 5 and MetaTrader 4 — featuring real-time calculations, risk visualization, and a modern trading dashboard.**

<br>

[![Stars](https://img.shields.io/github/stars/torvalds/linux?style=for-the-badge&color=00D4AA&label=Stars)](https://github.com/your-username/volume-profile-mt5/stargazers)
[![Forks](https://img.shields.io/github/forks/torvalds/linux?style=for-the-badge&color=4D9FFF&label=Forks)](https://github.com/your-username/volume-profile-mt5/network)
[![Issues](https://img.shields.io/github/issues/torvalds/linux?style=for-the-badge&color=FF4D6A&label=Issues)](https://github.com/your-username/volume-profile-mt5/issues)
[![Platform](https://img.shields.io/badge/MT5%20%2F%20MT4-Compatible-00D4AA?style=for-the-badge)](https://www.metatrader5.com)
[![License](https://img.shields.io/badge/License-MIT-4D9FFF?style=for-the-badge)](LICENSE)

</div>

---

## Screenshot

<div align="center">

![App Screenshot](assets/screenshot.png)

</div>

---

## Overview

**Position Sizer MT5/MT4** is a risk management tool designed for traders who want precise control over their positions.

Instead of guessing lot sizes, this tool calculates everything automatically based on your risk tolerance and trade setup.

It combines accurate calculation logic with a modern desktop interface inspired by professional trading platforms.

---

## What It Does

The application calculates optimal position sizing and visualizes trade risk in real time:

| Metric | Description |
|---|---|
| Lot Size | Automatically calculated based on risk and stop loss distance |
| Risk Amount | Exact dollar value at risk per trade |
| Reward Amount | Potential profit based on take profit level |
| Risk/Reward Ratio | Ratio between potential reward and risk |
| Stop Distance | Calculated in pips depending on instrument |
| Pip Value | Adjusted per symbol (Forex, Gold, JPY pairs) |

---

## Features

| Feature | Description |
|---|---|
| Real-Time Calculation | Instant updates when changing inputs |
| Multi-Asset Support | Forex pairs, Gold (XAUUSD), JPY pairs |
| Risk Slider | Fine-tune risk percentage interactively |
| BUY / SELL Modes | Direction-based calculations |
| Risk Meter | Visual gauge showing current risk level |
| Trade Simulation | Simulate trade execution and outcomes |
| Trade History | Track recent trades with results |
| Live Price Feed | Simulated real-time price movement |
| Modern UI | Dark themed trading dashboard |

---

## Interface

The application is structured into multiple panels:

- Sidebar — Navigation and system overview  
- Trade Parameters — Input values (balance, risk %, entry, SL, TP)  
- Results Panel — Lot size, risk, reward, R:R  
- Risk Meter — Visual gauge for risk exposure  
- Trade History — Executed trades with outcomes  

---

## Calculation Logic

```
Risk Amount = Account Balance × Risk %

Lot Size = Risk Amount / (StopLoss Pips × Pip Value)

Reward = Lot Size × TakeProfit Pips × Pip Value

R:R Ratio = Reward / Risk
```

---

## Risk Visualization

The built-in Risk Meter provides instant feedback:

- Low Risk → below 1.5%  
- Moderate Risk → 1.5% – 3%  
- High Risk → above 3%  

Color-coded feedback helps prevent overexposure.

---

## Quick Start

**Requirements:**
- Windows 10 / 11
- .NET 6+
- Visual Studio 2022

```bash
git clone https://github.com/your-username/position-sizer-mt5.git
```

Open the solution and run:

```
F5
```

No external dependencies required.

---

## How to Use

1. Enter account balance  
2. Set your risk percentage  
3. Define entry, stop loss, and take profit  
4. Choose BUY or SELL  
5. Review calculated lot size and R:R  
6. Use OPEN TRADE to simulate execution  
7. Track results in trade history  

---

## Designed for Trading

- Fast calculations  
- Clear visual feedback  
- Minimal and focused interface  

---

## Roadmap

- [ ] MT5 native integration (MQL5)
- [ ] MT4 version
- [ ] Real broker connection
- [ ] Auto trade execution
- [ ] Advanced analytics
- [ ] Export trade history

---

## Contributing

Pull requests are welcome.

```
1. Fork the repository
2. Create a branch
3. Commit changes
4. Open a pull request
```

---

## License

MIT License

---

<div align="center">

Position Sizer MT5/MT4 · Risk Management Tool · v1.0.0

</div>
