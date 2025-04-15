# 💱 Currency Converter 💵 ➡️ 💴

The Responsive Currency Converter is a web-based application built using HTML, CSS, and JavaScript. It allows users to seamlessly convert the currency of one country to another by fetching real-time exchange rates from an external API. With a simple and user-friendly interface, the tool ensures quick and accurate conversions, making it useful for travelers, shoppers, and anyone dealing with foreign currencies.

## 🎥 Project Demo

   Check out the live demo of the Currency Converter : [Demo](https://pratikkhot-currency-converter.netlify.app/)

---

## ✨ Features
- Convert currency values between different countries.
- Fetch real-time exchange rates using an API.
- Simple and user-friendly interface.

---

## 🛠 Tech Stack

- **HTML5** – Markup structure
- **CSS3** – Styling and responsive layout (Flexbox / Grid)
- **JavaScript (ES6+)** – Interactivity and API handling
- **API** – (e.g. OpenWeather, JSONPlaceholder, or your chosen one)

---

## 🖼️ Some Screenshots for the project:
 
 ![Screenshot 2025-04-15 004536](https://github.com/user-attachments/assets/e4269f89-f511-4600-8997-e5c6690c9075)

 ![Screenshot 2025-04-15 004152](https://github.com/user-attachments/assets/671b668a-f1c0-417d-a1cc-281be6a776eb)

---

## 📡 API Reference
```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/{fromcountry}.json
```

---

## 🔄 Fetching Exchange Rates
To fetch the exchange rates, the following code is used:

```bash
const BASE_URL = "https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies";
const url = `${BASE_URL}/${fromCurr.value.toLowerCase()}.json`;

let response = await fetch(url);
if (!response.ok) {
    throw new Error('Network response was not ok');
}

let data = await response.json();
const exchangeRate = data[fromCurr.value.toLowerCase()][toCurr.value.toLowerCase()];

```

---

## 📞 Contact Information

  🐙 GitHub: https://github.com/pratikkhot100

  💼 LinkedIn: https://www.linkedin.com/in/pratikkhot01

  📧 Email: pratikkhot1207@gmail.com
  
