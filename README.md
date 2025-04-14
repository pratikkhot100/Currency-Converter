# Currency Converter 💵 ➡️ 💴

This project is a Currency Converter built using HTML, CSS, and JavaScript. It allows users to convert the currency of one country to another by utilizing an external API.

## Project Demo

Check out the live demo of the Currency Converter: [Demo](https://pratikkhot100.github.io/Currency-Converter/)

---

## Features
- Convert currency values between different countries.
- Fetch real-time exchange rates using an API.
- Simple and user-friendly interface.

---

## API Reference
```
https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@latest/v1/currencies/{fromcountry}.json
```

---

## Fetching Exchange Rates
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
