# YNAB CLI with Streamlit Mirror

A simple command-line interface for YNAB (You Need A Budget) with a Streamlit web interface mirror. Manage your YNAB transactions through natural language commands!

## Features

- Natural language command processing
- Direct YNAB API integration
- Dual interface (CLI and web)
- Transaction validation
- Simple confidence scoring

## Setup

1. Clone the repository:
```bash
git clone [your-repo-url]
cd ynab-streamlit
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Create a `.env` file with your YNAB credentials:
```
YNAB_ACCESS_TOKEN=your_access_token
YNAB_BUDGET_ID=your_budget_id
```

## Usage

### CLI Mode
```bash
python main.py add 50 groceries to 2024-03-15
python main.py get accounts
```

### Streamlit Interface
```bash
streamlit run main.py
```

Then open your browser to the URL shown in the terminal.

## Command Examples

- Add transaction: `add [amount] [payee] to [YYYY-MM-DD]`
- Get data: `get [accounts|transactions]`

## Development

This is a garage project focused on simplicity and functionality. No complex databases, caching, or authentication - just pure Python and direct API calls! 