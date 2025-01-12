# 🌟 KoinX Backend Assignment 🌟

Welcome to the **KoinX Backend Assignment**! This project is a backend service designed to analyze cryptocurrency data by fetching real-time data from CoinGecko and providing valuable statistics.

## 🚀 Features

- **Regular Data Fetching**: Fetch cryptocurrency data at regular intervals and store it for analysis.
- **Cryptocurrency Statistics**: Get the latest price, market capitalization, and standard deviation for your favorite cryptocurrencies.

---

## 🛠️ Technology Stack

- **Node.js**: Powering the backend and API logic.
- **Express.js**: Simplifying API creation and HTTP request handling.
- **MongoDB**: Storing cryptocurrency data for fast access and analysis.
- **CoinGecko API**: Fetching the most accurate and up-to-date cryptocurrency data.

---

## 🧑‍💻 API Endpoints

### 1️⃣ Get Cryptocurrency Stats

- **Endpoint**: `/api/v1/crypto/stats`
- **Method**: `GET`
- **Purpose**: Fetch key stats like price, market cap, and supply for a specified cryptocurrency.

#### Request Body Example:
```json
{
  "coin": "bitcoin"
}
```

#### 📥 Example Request:
```bash
GET https://koinx-backend-eq0e.onrender.com/api/v1/crypto/stats
BODY: {"coin": "bitcoin"}
```

#### 📤 Example Response:
```json
{
  "coin": "bitcoin",
  "latest_price": 45000,
  "market_cap": 850000000000,
  "circulating_supply": 18500000
}
```

---

### 2️⃣ Get Price Deviation

- **Endpoint**: `https://koinx-backend-eq0e.onrender.com/api/v1/crypto/deviation`
- **Method**: `GET`
- **Purpose**: Fetch the standard deviation of a cryptocurrency's price over a specific time period.

#### Request Body Example:
```json
{
  "coin": "ethereum"
}
```

#### 📥 Example Request:
```bash
GET https://koinx-backend-eq0e.onrender.com/api/v1/crypto/deviation
BODY: {"coin": "ethereum"}
```

#### 📤 Example Response:
```json
{
  "coin": "ethereum",
  "price_deviation": 2000
}
```

---

## 💻 How to Run the Project

### 📝 Prerequisites

1. [Node.js](https://nodejs.org/) installed on your machine.
2. [MongoDB](https://www.mongodb.com/try/download/community) (or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for cloud-based storage).
3. A **CoinGecko API** key for fetching cryptocurrency data (if needed).

---

### 🚀 Running the Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-repository/koinx-backend-assignment.git
   ```

2. **Navigate into the project directory:**
   ```bash
   cd koinx-backend-assignment
   ```

3. **Install required dependencies:**
   ```bash
   npm install
   ```

4. **Set up your environment variables:**
   Create a `.env` file with the necessary configuration, such as MongoDB URI and CoinGecko API key.

5. **Start the server:**
   ```bash
   npm start
   ```

   By default, the backend will be available at `http://localhost:5000`.

---

## 🎨 Visuals

![Crypto Stats](https://i.imgur.com/ZdCzSlT.png)

---

## 🤝 Contributing

We welcome contributions from anyone! Feel free to open an issue, create a pull request, or offer any suggestions.

### Steps to Contribute:
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a new Pull Request.

---

## 📜 License

This project is open-source and licensed under the [MIT License](LICENSE).

---

## 🛠️ Troubleshooting

Having issues? Here are a few tips to resolve common problems:

- **API Not Fetching Data**: Double-check your CoinGecko API key in `.env`.
- **Database Connection Failed**: Ensure MongoDB is running, and check the MongoDB URI configuration.
