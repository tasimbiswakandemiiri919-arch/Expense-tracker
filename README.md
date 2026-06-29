

---

# SpendWise — Expense Tracker

A sleek, modern expense tracking application built with vanilla HTML, CSS, and JavaScript. Track your income and expenses with beautiful visualizations and local storage persistence.

## Features

### 📊 Dashboard
- **Net Balance**: Real-time overview of your financial health
- **Income & Expenses**: Track totals with transaction counts
- **Savings Rate**: See what percentage of income you're saving
- **Monthly Filtering**: Switch between months to analyze trends

### 💰 Transaction Management
- **Add Transactions**: Quick form for income and expenses
- **Categories**: Pre-defined categories with emoji icons (Food, Transport, Housing, etc.)
- **Filtering**: View all, income-only, or expense-only transactions
- **Delete**: Remove unwanted transactions with one click
- **Persistence**: All data stored in browser's localStorage

### 📈 Visual Analytics
- **Spending by Category**: Donut chart showing expense distribution
- **Income vs Expenses**: Bar chart comparing last 6 months
- **Budget Bars**: Top spending categories with percentage breakdown
- **Responsive**: Works on desktop and mobile devices

## Technologies Used

- **HTML5**: Semantic structure
- **CSS3**: Custom properties, flexbox, grid, animations
- **JavaScript (ES6)**: Vanilla JS, no frameworks
- **Chart.js v4.4.1**: Beautiful, interactive charts
- **Google Fonts**: JetBrains Mono & Inter typography
- **LocalStorage**: Client-side data persistence

## Installation

1. **Clone or download** the `expense-tracker.html` file
2. **Open in browser**: Simply double-click the file or open with your favorite browser
3. **No server needed**: Works completely offline!

## Usage Guide

### Adding a Transaction
1. Select **Income** or **Expense** using the toggle buttons
2. Fill in the details:
   - **Description**: Brief note about the transaction
   - **Amount**: Dollar amount (positive numbers only)
   - **Category**: Choose from relevant categories
   - **Date**: Defaults to today
3. Click **Add Income/Expense** to save

### Viewing Data
- **Month Selector**: Top-right dropdown to view different months
- **Transaction Filter**: Use "All", "Income", or "Expenses" buttons
- **Delete**: Hover over a transaction and click the ✕ button

### Understanding Statistics
- **Net Balance**: Income minus expenses (shows +/-)
- **Savings Rate**: (Balance ÷ Income) × 100
- **Categories**: Color-coded for easy identification

## Data Structure

Transactions are stored with the following schema:
```json
{
  "id": 1234567890,
  "desc": "Freelance Payment",
  "amount": 350.00,
  "type": "income",
  "category": "freelance",
  "date": "2026-06-29"
}
```

## Customization

### Categories
Edit the `CATEGORIES` object in the JavaScript to add or modify categories:
```javascript
const CATEGORIES = {
  income: [
    {id:'salary', label:'Salary', icon:'💼', color:'#68d391'},
    // Add your own...
  ],
  expense: [
    {id:'food', label:'Food', icon:'🍔', color:'#fc8181'},
    // Add your own...
  ]
};
```

### Colors
Modify the CSS custom properties in `:root`:
```css
:root {
  --bg: #0a0f1e;
  --accent: #63b3ed;
  --green: #68d391;
  --red: #fc8181;
  /* ... */
}
```

## Responsive Design

The application automatically adapts to:
- **Desktop**: Full dashboard with sidebar
- **Tablet**: Collapsed layout
- **Mobile**: Stacked cards, simplified navigation

## Browser Support

Works on all modern browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Limitations

- **Client-side only**: Data lives in your browser (localStorage)
- **No cloud sync**: Clearing browser data will remove transactions
- **Single currency**: USD by default (can be changed in code)
- **No export**: Consider adding CSV export for backups

## Future Improvements

- [ ] CSV/JSON export functionality
- [ ] Dark/light theme toggle
- [ ] Recurring transactions
- [ ] Budget limits & alerts
- [ ] Goal setting features
- [ ] Multi-currency support
- [ ] Transaction search
- [ ] Data backup/restore

## License

MIT License - Feel free to use, modify, and distribute as needed.

## Credits

**Developer & Designer**
- **Tasimbiswa Kandemiiri**
- Year 2 Student at **TelOne Center For Learning**
- Harare, Zimbabwe

**Third-Party Libraries**
- **Chart.js**: For beautiful chart visualizations
- **Google Fonts**: For the typography

**Special Thanks**
- All users and contributors who help make SpendWise better

---

**Made with ❤️ by Tasimbiswa Kandemiiri • TelOne Center For Learning, Harare, Zimbabwe**
