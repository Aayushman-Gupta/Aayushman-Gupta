# 📊 Live Stock Price Simulator & Dashboard

A **real-time stock dashboard** built with **React + Vite**, streaming stock prices over **WebSockets** and visualized using **Recharts**.  
If the WebSocket server is unavailable, the app gracefully switches to **mock data mode** so the UI always stays alive.

---

## ✨ Features

- ⚡ **Real-time WebSocket Streaming** – Live stock updates with every tick  
- 🎨 **Dark-Themed Modern UI** – Responsive dashboard styled with **TailwindCSS**  
- 📈 **Interactive Charts** – Area & line charts with smooth curves, shaded trends, tooltips, and legends  
- 📉 **20-Period Moving Average** – Overlayed on stock charts for trend analysis  
- 🔄 **Automatic Mock Fallback** – Backend down? Generates realistic random stock data  
- 📱 **Responsive Design** – Works seamlessly on desktop, tablet, and mobile  

---

## 🖼️ Demo Preview

<p align="center">
  <img src="demo/dashboard.png" alt="Dashboard Preview" width="49%">
  <img src="demo/stock-cards.png" alt="Stock Cards" width="49%">
</p>

---

## 🛠️ Tech Stack

### Frontend
- ⚛️ [React](https://reactjs.org/) (via [Vite](https://vitejs.dev/)) – Lightning-fast development  
- 🎨 [TailwindCSS](https://tailwindcss.com/) – Utility-first styling  
- 📊 [Recharts](https://recharts.org/) – Beautiful charts  

### Backend
- 💻 C++ Stock Simulator  
- 🔌 WebSocket server at `ws://localhost:9002`  

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/stock-price-simulator.git
cd stock-price-simulator
