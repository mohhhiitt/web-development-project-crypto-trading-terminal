# web-development-project-crypto-trading-terminal
# 💹 CryptoTerminal — Crypto Trading Terminal Webpage

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Complete-00ff88?style=for-the-badge)

> A beginner-friendly **crypto trading terminal** webpage built with pure HTML, CSS, and JavaScript — no frameworks, no libraries, just one single file.

---

## 📸 Preview

```
💹 CryptoTerminal        Home  Markets  Portfolio  Login
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📊 Live Crypto Prices
[ 🔄 Refresh Prices ]

┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
│  ₿ Bitcoin  │  │ Ξ Ethereum  │  │  ◎ Solana   │  │    B BNB    │
│  $67,431    │  │   $3,821    │  │    $185     │  │    $612     │
│  ▲ +2.3%   │  │  ▲ +1.8%   │  │  ▼ -0.9%   │  │  ▲ +0.4%   │
└─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘
```

---

## ✨ Features

- 🌑 **Dark theme** — professional trading terminal look
- 📊 **4 Crypto cards** — Bitcoin, Ethereum, Solana, BNB
- 🔄 **Refresh button** — simulates live price updates
- 🟢 **Green ▲** for price up / 🔴 **Red ▼** for price down
- 🧭 **Navigation bar** — Home, Markets, Portfolio, Login
- 📁 **Single file** — everything in one `index.html`

---

## 🗂️ Project Structure

```
crypto-terminal/
│
└── 📄 index.html        ← All code (HTML + CSS + JavaScript)
```

---

## 🛠️ Tech Stack

| Technology | Usage |
|:----------:|-------|
| **HTML5** | Page structure — navbar, cards, button, footer |
| **CSS3** | Styling — dark theme, flexbox layout, hover effects |
| **JavaScript** | Logic — random price generation, DOM updates |

---

## ⚡ Getting Started

### 🔁 Clone this Repository

```bash
git clone https://github.com/your-username/crypto-terminal.git
cd crypto-terminal
```

### ▶️ Run the Project

**Option 1 — VS Code + Live Server (Recommended)**

1. Install [VS Code](https://code.visualstudio.com/)
2. Install the **Live Server** extension by *Ritwick Dey*
3. Open the project folder in VS Code
4. Right-click `index.html` → click **"Open with Live Server"**
5. Browser opens automatically ✅

**Option 2 — Direct Open**

1. Download or clone the repo
2. Double-click `index.html`
3. Opens in your browser instantly ✅

---

## 🧠 How the Code Works

### 1️⃣ HTML — Page Structure
```html
<!-- One price card -->
<div class="card">
  <div class="coin-name">₿ Bitcoin</div>
  <div class="coin-price" id="btc-price">$67,431</div>
  <div class="up" id="btc-change">▲ +2.3%</div>
</div>
```

### 2️⃣ CSS — Dark Styling
```css
body  { background-color: #0a0a0a; color: white; }
.card { background-color: #1a1a1a; border-radius: 10px; }
.up   { color: #00ff88; }   /* Green */
.down { color: #ff4444; }   /* Red   */
```

### 3️⃣ JavaScript — Price Logic
```javascript
function updatePrices() {
  // Generate a random price near $67,000
  let btcPrice = 67000 + Math.floor(Math.random() * 2000);

  // Update the HTML element with the new price
  document.getElementById("btc-price").innerText = "$" + btcPrice;
}
```

---

## 📌 JavaScript Concepts Used

| Concept | Description |
|---------|-------------|
| `Math.random()` | Generates a random decimal number |
| `Math.floor()` | Rounds down to a whole number |
| `getElementById()` | Selects an HTML element by its ID |
| `.innerText` | Updates the visible text on the page |
| `.className` | Switches CSS class for color change |
| `if / else` | Checks if price went up or down |
| `toFixed(2)` | Rounds a number to 2 decimal places |

---

## 🔮 Future Improvements

- [ ] Connect to **CoinGecko API** for real live prices
- [ ] Add a **price history chart** using Chart.js
- [ ] Add **search bar** to look up any coin
- [ ] Make it **mobile responsive**
- [ ] Add a **Buy / Sell** order panel
- [ ] Add **dark/light mode** toggle

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**mohit jaiswal **  
GitHub: [@your-username](https://github.com/your-username)

---

> ⭐ If you found this project helpful, please give it a **star** on GitHub
