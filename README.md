# GigShield

AI-powered parametric income insurance platform for gig delivery partners in India.

## 🛡️ Features

- **PWA Ready**: Install as a mobile or desktop app for offline use.
- **Dynamic Risk Map**: Real-time monitoring of weather and platform risks across 300+ Indian cities.
- **Parametric Triggers**: Automated payouts based on IMD data (Rain, Heat, AQI).
- **AI Fraud Guard**: Smart validation of claims using motion and location sensors.

## 🚀 One-Click Deployment (Railway)

GigShield is pre-configured for direct deployment on [Railway.app](https://railway.app/).

### Quick Deploy:
1. Connect your GitHub repository to Railway.
2. The platform will automatically detect the `package.json` and start the server.
3. **Mandatory Configuration**: 
   - Navigate to **Settings > Variables**.
   - Add `GEMINI_API_KEY`: Your Google AI API key.
   - Add `PORT`: `3000` (optional, Railway will assign its own if not provided).

### 💾 Persistent Storage
By default, the SQLite database (`database.sqlite`) is **ephemeral**. 
To persist user data:
- Go to Railway settings for your service.
- Click **Volumes > New Volume**.
- Mount it at `/app/database.sqlite`.

---

## 💻 Local Development

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the dev server:
   ```bash
   npm run dev
   ```
3. Open `http://localhost:3000`.

## 🛠️ Technology Stack

- **Frontend**: Vanilla JS, HTML5, CSS3 (Glassmorphism design language).
- **Backend**: Node.js, Express.
- **Database**: SQLite3.
- **AI**: Google Gemini Pro (via Backend Proxy).
