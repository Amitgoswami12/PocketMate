# PocketMate 💳

A **credit card recommendation web app** built with **Node.js, Express, EJS and MongoDB**. Users browse top credit card picks, compare interest rates and features (travel, rewards, insurance, entertainment), and get cards suggested for their preferences.

![Node.js](https://img.shields.io/badge/Node.js-Express-339933?logo=nodedotjs&logoColor=white)
![EJS](https://img.shields.io/badge/EJS-templates-B4CA65)
![MongoDB](https://img.shields.io/badge/MongoDB-Mongoose-47A248?logo=mongodb&logoColor=white)

## ✨ Features

- **Top picks:** a card gallery built from a credit-card dataset, showing name, interest rate and key features.
- **Recommendations:** fill in a preference form and get suggested cards on the `/recommend` page.
- **Score page:** a questionnaire flow (`/sat_score` → `/s_score`).
- **User model:** Mongoose schema for users with saved cards.
- **Server-rendered UI:** EJS views with shared layouts (`express-ejs-layouts`) and Bootstrap navigation.

## 🏗️ Structure

```
├── server.js              Express app and routes
├── dbConnect.js           MongoDB connection (reads MONGO_URI from .env)
├── schema.js              User model (username, password, savedCards)
├── credit_card_data.json  Card dataset (name, interest, features)
├── views/                 EJS pages: index, top_picks, rec, recommend, sat_score …
└── public/                CSS
```

## 🚀 Run locally

```bash
git clone https://github.com/Amitgoswami12/NodeJS.git
cd NodeJS
npm install
```

Create a `.env` file:

```env
Mongo_URI=your-mongodb-connection-string
```

Start the app:

```bash
npm start        # nodemon server.js
```

## 🔭 Roadmap

- Replace the fixed recommendation list with a scoring engine based on the user's form answers.
- Add login with hashed passwords and a "Saved cards" page.

## 👤 Author

**Amit Goswami** · [Portfolio](https://amitgoswami12.github.io) · [GitHub](https://github.com/Amitgoswami12)
