# 🪙 Karat Quotes: Live Indian Gold Rate Tracker

A sleek, real-time web dashboard tracking Indian market gold prices across all karats. Designed with a premium, responsive UI, it calculates live spot rates, applies local market premiums, and tracks daily price deltas.

![Gold Rate UI Screenshot](https://github.com/themaulik/Today-Gold-Rate/blob/main/Today-Gold-Rate.png?raw=true)

## ✨ The Hallmarks (Features)

* **📈 Live Spot Pricing:** Fetches real-time international gold data and converts it directly to INR.
* **🇮🇳 Indian Market Premium:** Automatically applies a ~15% markup to reflect actual local bullion market rates, import duties, and taxes.
* **🏅 Multi-Karat Display:** Showcases accurate pricing for 24K (Pure), 22K (Hallmark), 20K (Premium), 18K (Classic), 14K (Light), and 9K (Entry) gold.
* **📊 Daily Delta Tracking:** Calculates and displays the exact price difference and percentage change compared to the previous day's closing rate.
* **💾 Persistent Memory:** Uses local storage to remember daily price logs, ensuring the "vs yesterday" metric is always accurate.
* **📱 Elegant & Responsive:** Features a beautiful dark-mode "Hero" card for the most popular 22K gold, fluid grid layouts, and the crisp Manrope typography.

## 🧪 The Alchemy (Tech Stack)

* **Core:** Pure HTML5, CSS3, and Vanilla JavaScript (Zero dependencies).
* **Data Sources:** 
  * `api.gold-api.com` for live XAU/INR spot prices.
  * `open.er-api.com` for fallback currency conversion rates.
* **Storage:** Browser `localStorage` (via custom wrapper) for historical daily price tracking.

## ⚙️ The Minting Process (How It Works)

1. **The Pour:** The app fetches the live international spot price of gold in USD and the current USD to INR exchange rate.
2. **The Alloy:** It calculates the base price per gram in INR and applies a **1.15x multiplier** to simulate the Indian retail market premium (covering import duties and local jeweler margins).
3. **The Stamping:** The base 24K price is multiplied by the specific purity ratios (e.g., 0.916 for 22K, 0.833 for 20K) to generate accurate cards for every karat.
4. **The Ledger:** It checks the local storage ledger to find the last recorded price from a previous day, calculates the delta, and updates the UI with green (up) or red (down) indicators.

## 🚀 Unlocking the Vault (Setup & Deployment)

### Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/themaulik/Today-Gold-Rate.git
