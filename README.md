# 💱 Currency Converter (React + Custom Hook)

A modern Currency Converter built using **React** and a custom hook `useCurrencyInfo` for fetching and managing real-time exchange rate data.

This project demonstrates clean component architecture, reusable hooks, and proper separation of concerns.

---

## 🚀 Features

- Convert between multiple currencies
- Real-time exchange rate fetching
- Swap currencies instantly
- Controlled inputs
- Custom reusable React Hook (`useCurrencyInfo`)
- Clean and modular component structure

---

## 🏗️ Architecture Overview

The application follows a modular and scalable React architecture:

src/
├── components/
│ └── InputBox.jsx
├── hooks/
│ └── useCurrencyInfo.js
├── App.jsx
├── main.jsx


### 🔹 Core Design Principles

- **Separation of Concerns**
- **Reusable Hook Logic**
- **Unidirectional Data Flow**
- **Controlled Components**
- **Functional Components with Hooks**

---

## 🧠 Custom Hook: `useCurrencyInfo`

The core logic of exchange rate fetching is abstracted into a custom hook:

```js
useCurrencyInfo(baseCurrency)
```
--- 

## Responsibilities:

- Fetch currency data from API

- Return exchange rates object

- Re-fetch when base currency changes

- Encapsulate side-effects using useEffect

--- 

## Why Use a Custom Hook?

- Promotes code reuse

- Improves readability

- Keeps App.jsx clean

- Scales better in larger applications

---

## 🔄 Conversion Flow

- User enters amount

- User selects base currency

- useCurrencyInfo(baseCurrency) fetches rates

- Converted amount is calculated

- UI updates reactively