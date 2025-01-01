# portfoliotracker-stock
Portfolio Tracker

Overview
The Portfolio Tracker is a full-stack application that helps users track their stock investments. Users can add, view, and delete stocks while seeing real-time stock price updates, total portfolio value, and total investment value. The application uses React for the frontend, Node.js with Express for the backend, and MongoDB as the database.
Steps to Run the Project Locally
Prerequisites
Node.js installed (v14 or above recommended)
MongoDB Atlas account or a local MongoDB setup
A Finnhub API key
Backend Setup
Clone the repository
git clone <repository-url>
cd <repository-directory>

Install backend dependencies
cd backend
npm install
Set up environment variables
Create a .env file in the backend directory with the following keys:
MONGODB_USERNAME=<your-mongodb-username>
MONGODB_PASSWORD=<your-mongodb-password>
FINNHUB_API_KEY=<your-finnhub-api-key>
Start the backend server
npm start
The backend server will run on http://localhost:5000 by default.
Frontend Setup
Navigate to the frontend directory
cd frontend
Install frontend dependencies
npm install
Update backend URL
Ensure the BACKEND_URL in frontend/src/App.js is set to your local backend URL:
const BACKEND_URL = "http://localhost:5000";
Start the frontend application
npm start
The frontend will run on http://localhost:3000 by default.
Assumptions and Limitations
Assumptions
The Finnhub API key provided has sufficient credits for API calls.
All stocks added have valid tickers that are recognized by Finnhub.
The MongoDB database is set up correctly with user credentials.
Limitations
Real-time updates depend on Finnhub API limits and response times.
API rate limits may delay or block stock data retrieval.
Stocks are stored with a default quantity of 1.
Deployed backend might face higher latency compared to local testing.
Links

Deployed Application
https://stock-portfolio-nithin.netlify.app/
Live API Documentation
https://backend-stock-t8a3.onrender.com

