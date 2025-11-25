# Personal Finance Manager

A full-stack application to track personal finances with a Windsurf frontend and Python FastAPI backend.

## Features

- Add income and expense transactions with date, amount, category, and description
- View transaction history
- See financial summaries (total income, expenses, savings)
- Visualize expenses by category
- Responsive design

## Setup

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment (recommended):
   ```bash
   python -m venv venv
   .\venv\Scripts\activate  # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the backend server:
   ```bash
   python main.py
   ```
   The API will be available at `http://localhost:8000`

### Frontend Setup

1. Install Windsurf CLI (if not already installed):
   ```bash
   npm install -g windsurf-cli
   ```

2. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

3. Run the Windsurf development server:
   ```bash
   windsurf dev
   ```
   The frontend will be available at `http://localhost:3000`

## API Endpoints

- `GET /` - Welcome message
- `GET /transactions` - Get all transactions
- `POST /transactions` - Create a new transaction
- `GET /transactions/summary` - Get financial summary

## Data Storage

All transaction data is stored in `backend/finance_data.json`
