# Crypto Volatility Watcher

An institutional-grade market monitoring system that identifies and logs significant cryptocurrency price movements. This project bridges a high-fidelity **Lovable** frontend with a robust **Make.com** automation backend.

## 🚀 Overview

The **Crypto Volatility Watcher** is designed to filter market noise. Instead of manual tracking, it uses automated logic to detect when a top-tier cryptocurrency experiences a price swing of $\ge 5\%$ within a 24-hour window.

## 🛠️ System Architecture

* **Frontend:** [Lovable](https://lovable.dev) (React/Vite) – A professional "Enterprise Navy" dashboard for system interaction.
* **Automation Engine:** [Make.com](https://make.com) – The central "brain" handling logic, API requests, and data routing.
* **Data Source:** [CoinGecko API](https://www.coingecko.com/en/api) – Industry-standard real-time market data.
* **Database/Logging:** [Google Sheets](https://sheets.google.com) – Persistent storage for all triggered volatility alerts.

## 🧠 Technical Workflow

1.  **User Trigger:** The user initiates a scan via the "Trigger Market Scan" button on the Lovable UI.
2.  **Webhook Communication:** The frontend sends a `POST` request to a secure **Make.com Webhook**.
3.  **Data Acquisition:** Make.com calls the **CoinGecko API** to retrieve current market data for the top 100 assets.
4.  **Volatility Logic:** The system iterates through the data and applies a numeric filter to identify assets with a 24h change $\ge 5\%$ or $\le -5\%$.
5.  **Logging:** Successfully filtered assets are appended to a **Google Sheet** with a unique timestamp, current price, and percentage change.

## 🎨 UI/UX Design

The dashboard follows a "Professional Financial Terminal" aesthetic:
* **Theme:** Deep Navy (`#0f172a`) with high-contrast content cards.
* **Feedback:** Real-time button loading states ("Scanning...") and success toast notifications.
* **Precision:** Monospace font styling for all financial values to ensure maximum readability.

## 📸 Media & Demos

### Dashboard Screenshot
![Dashboard Screenshot]
<img width="1366" height="768" alt="Screenshot (217)" src="https://github.com/user-attachments/assets/7814f66b-9acf-4c72-babf-62581029e01c" />
<img width="1366" height="768" alt="Screenshot (214)" src="https://github.com/user-attachments/assets/ce82e61d-dfbe-4fe7-a79a-50a5f6394ed2" />
<img width="1366" height="768" alt="Screenshot (211)" src="https://github.com/user-attachments/assets/26cec592-8409-45df-8feb-d23fb2b993f4" />



### Video Walkthrough
[📺 Watch the Live Demo]


https://github.com/user-attachments/assets/a3d177e3-9d71-4544-ad50-9a972c7a9fc4


### Built by Snazzy-devv

## 📁 Repository Structure

```plaintext
├── src/                # Lovable/React frontend components
├── public/             # Static assets (icons, images)
├── docs/               # Technical PRD and workflow diagrams
└── README.md           # Project documentation



