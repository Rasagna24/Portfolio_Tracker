# 📊 Google Sheets Portfolio Tracker

A personal stock portfolio tracker built using Google Sheets — designed to help investors monitor their holdings, calculate real-time returns, and visualize their investment performance.

---

## 💡 What It Does

This spreadsheet helps you:
- Track stock tickers, quantities, buy prices, and current prices
- Automatically calculate:
  - Total Invested
  - Current Value
  - Gain/Loss ₹
  - % Return
- Visualize your portfolio with:
  - Pie chart (based on total investment allocation)
  - Bar chart (gain/loss per stock)

---

## 🧰 How to Use

1. Open the Google sheet 
   _or download `Portfolio_Tracker_Template.xlsx` from this repo_

2. Manually update the **Current Price** (or use `=GOOGLEFINANCE()` in Google Sheets only)

3. The formulas will auto-calculate:
   - `Total Invested = Buy Price × Quantity`
   - `Current Value = Current Price × Quantity`
   - `Gain/Loss = Current Value − Total Invested`
   - `% Return = Gain/Loss ÷ Total Invested`

4. Check the charts below the data to visualize your performance

---

## 🖼️ Preview

<img width="1286" height="735" alt="image" src="https://github.com/user-attachments/assets/c521633b-c6f1-4c2d-b98d-786c7c213ac0" />


---

## 🔧 Formulas Used

=GOOGLEFINANCE("TICKER", "price")        // For live market price (Google Sheets only)
=Buy Price × Quantity
=Current Price × Quantity
=Current Value − Total Invested
=(Gain/Loss ÷ Total Invested)

## 📌 Features

- Live price fetching with `GOOGLEFINANCE()` (Google Sheets only)
- Automatic gain/loss + % return calculation
- Clean, visual charts (Pie + Bar)
- Easy to customize and expand

## 🛠️ Upcoming Improvements (To-Do)

- Add a dashboard for top gainers/losers
- Support for dividends & SIP tracking
- Python automation version

