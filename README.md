# CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2
```markdown
# 📈 Stock Portfolio Tracker

> **CodeAlpha Python Programming Internship – Task 2**  
> A console‑based tool to calculate your total investment value using hardcoded stock prices, with a numbered menu, input validation, and optional CSV export.

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with Colab](https://img.shields.io/badge/Made%20with-Colab-orange)](https://colab.research.google.com/)

---

## 📖 Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Demo](#demo)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

---

## 📌 Project Description

The **Stock Portfolio Tracker** is a Python application that helps users quickly calculate the total value of their stock holdings. Instead of entering stock symbols manually, users select from a numbered menu of predefined stocks (AAPL, TSLA, GOOGL, MSFT, AMZN, META). For each chosen stock, the user inputs the number of shares, and the program computes the current value using hardcoded prices. The portfolio is displayed in a formatted table, and the user can optionally save the summary as a CSV file.

The application is designed to run in **Google Colab** or any Python terminal, using only the standard library (no external dependencies).

---

## ✨ Features

- **Predefined stock prices** – six well‑known stocks with realistic prices.
- **Numbered menu** – select stocks by number (no typing errors).
- **Input validation** – ensures positive integer shares and valid selections.
- **Formatted portfolio table** – shows symbol, shares, price, and value.
- **Investment summary** – total value, largest and smallest holding.
- **Coloured console output** (green for success, red for errors, cyan for headings).
- **Save to CSV** – optional export with a timestamped filename.
- **Automatic download** in Colab (via `files.download()`).
- **Menu‑driven loop** – enter, view, save, exit without restarting.

---

## 🛠 Tech Stack

| Category         | Tools / Libraries                        |
| ---------------- | ---------------------------------------- |
| **Language**     | Python 3.8+                              |
| **Environment**  | Google Colab / any terminal              |
| **Standard libs**| `csv`, `datetime`, `os`, `zipfile` (for packaging) |
| **No third‑party dependencies** | –                         |

---

## 📁 Project Structure

```
CodeAlpha_Stock_Portfolio_Tracker/
├── stock_portfolio_tracker.py    # Main Python script
├── Stock_Portfolio_Tracker.ipynb # Colab notebook (optional)
├── README.md                     # This file
├── requirements.txt              # (empty – no dependencies)
└── stock_tracker_results/        # Output folder (saved CSV files, sample output)
    └── portfolio_YYYYMMDD_HHMMSS.csv
```

---

## 🚀 Installation & Setup

### Option 1: Google Colab (Recommended – no setup)

1. Open the notebook in Colab:  
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/shaikhdaiyaan251-cloud/CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2/blob/main/Stock_Portfolio_Tracker.ipynb)

2. Run the cells sequentially. The first cell sets up colours and stock data.

3. Follow the interactive menu.

### Option 2: Local Python environment

1. Clone the repository:
   ```bash
   git clone https://github.com/shaikhdaiyaan251-cloud/CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2.git
   cd CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2
   ```

2. Run the script:
   ```bash
   python stock_portfolio_tracker.py
   ```

No extra installation is required.

---

## 💻 Usage

When you run the program, you will see a main menu:

```
💰 STOCK PORTFOLIO TRACKER
========================================
1. Enter/Update Portfolio
2. View Portfolio
3. Save Portfolio
4. Exit
👉 Choose (1-4):
```

- **Option 1** – Enter your holdings. You will be asked how many different stocks you own, then for each stock you select a number from the menu and input shares.

- **Option 2** – Display the current portfolio in a formatted table, along with the total value and largest/smallest holdings.

- **Option 3** – Save the portfolio to a CSV file. The file is automatically named with a timestamp and (in Colab) downloaded to your computer.

- **Option 4** – Exit the program.

### Example session (Option 1)

```
📋 AVAILABLE STOCKS
Symbol       Price
--------------------
AAPL       $180.25
TSLA       $250.50
GOOGL      $140.30
MSFT       $330.00
AMZN       $128.50
META       $310.75

📝 Let's build your portfolio.
How many different stocks do you own? 2

--- Stock #1 ---
👉 Select stock by number: 1
Enter number of shares for AAPL: 10
✅ Added 10 shares of AAPL @ $180.25 = $1,802.50

--- Stock #2 ---
👉 Select stock by number: 2
Enter number of shares for TSLA: 5
✅ Added 5 shares of TSLA @ $250.50 = $1,252.50
```

Then viewing the portfolio (Option 2) gives:

```
📊 YOUR PORTFOLIO SUMMARY
Symbol    Shares       Price         Value
--------------------------------------------------
AAPL          10     $180.25     $1,802.50
TSLA           5     $250.50     $1,252.50
--------------------------------------------------
TOTAL                         $3,055.00

📈 INVESTMENT SUMMARY
   Number of holdings: 2
   Total invested value: $3,055.00
   Largest holding: AAPL ($1,802.50)
   Smallest holding: TSLA ($1,252.50)
```

---

## 🖼️ Demo

![Demo Screenshot Placeholder](stock_tracker_results/sample_output.txt)  
*(Replace with actual screenshot or use the sample output file provided.)*

---

## 🔮 Future Improvements

- **Real‑time prices** – integrate an API like Yahoo Finance or Alpha Vantage to fetch live prices.
- **Add / remove holdings** – edit portfolio without re‑entering everything.
- **Profit / loss calculation** – store purchase prices and show gain/loss.
- **Web interface** – build a simple dashboard using Streamlit or Flask.
- **Portfolio charts** – pie chart of holdings distribution.

---

## 🤝 Contributing

Contributions are welcome! If you have an idea or find a bug:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/amazing-feature`).
3. Commit your changes (`git commit -m 'Add some amazing feature'`).
4. Push to the branch (`git push origin feature/amazing-feature`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

## 🙏 Acknowledgements

- **CodeAlpha** – for the internship opportunity.
- Python’s standard library – keeping things simple and dependency‑free.

---

## 📬 Contact

**DAIYAAN SHAIKH** – [LinkedIn](https://www.linkedin.com/in/daiyaan-shaikh-159909377?utm_source=share_via&utm_content=profile&utm_medium=member_android) – [GitHub](https://github.com/shaikhdaiyaan251-cloud)  

Project Link: [[https://github.com/shaikhdaiyaan251-cloud/CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2](https://github.com/shaikhdaiyaan251-cloud/CODE-ALPHA-PYTHON-PROGRAMMING-INTERNSHIP-TASK-2)]


---

⭐ **If this tool helps you track your investments, please give it a star!** ⭐
```
