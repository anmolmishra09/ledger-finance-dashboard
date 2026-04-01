Ledger — Finance Dashboard

A clean, interactive personal finance dashboard built as a single self-contained HTML file with no build step and no dependencies required.

This project demonstrates how a full-featured dashboard can be built using pure HTML, CSS, and Vanilla JavaScript.

🚀 Quick Start
Option 1 — Open directly
open finance-dashboard.html
Option 2 — Run a local server (recommended)
npx serve .

or

python3 -m http.server 8080

That's it — no npm install, no bundler, no backend needed.

📋 Features
1. Dashboard Overview
Summary Cards
Total Balance (all-time net)
Monthly Income
Monthly Expenses
Savings Rate with comparison to previous month
Balance Trend Chart
SVG line + area chart
Shows income vs expenses across the last 6 months
Spending Donut Chart
Expense category breakdown
Live percentage legend
Recent Activity
Displays the last 5 transactions
2. Transactions Section

Full transaction management interface:

Transaction table includes:
Date
Description
Category
Type
Amount
Search
Real-time filtering
Filters
Income / Expense
Category
Month
Sorting
Date
Amount
Category
Type
Export CSV
Download filtered transaction data
3. Role-Based UI (Frontend Simulation)

Switch roles using the badge in the top-right corner.

Role	Access
Viewer	Read-only
Admin	Full control
Viewer Mode
Can browse transactions
Can search and filter
Can export data
Admin Mode
Add transactions
Edit transactions
Delete transactions

Role switching happens instantly without login.

4. Insights Section

Advanced financial insights including:

Top Spending Category
Top 5 category ranking
Monthly income vs expense comparison
Auto-generated financial observations
Income vs Expense ratio visualization
🧠 State Management

All data is stored inside a single state object:

{
  transactions: [...],
  role: "viewer",
  theme: "dark",
  nextId: 100
}

The state is automatically saved to localStorage, so data persists after page refresh.

✨ UX Features
Dark / Light theme toggle
Responsive design
Mobile-friendly layout
Collapsible sidebar
Empty state handling
Toast notifications
Smooth animations
Modal transitions
Adaptive tables
🗂 Project Structure

Everything exists in one file:

finance-dashboard.html
│
├── <style>     CSS variables, layout, components
├── HTML        Sidebar, dashboard pages, modal
└── <script>    State, rendering logic, charts, CRUD
Architecture
Render-on-demand UI
Vanilla JavaScript state updates
Inline SVG charts
DOM-based filters
🛠 Assumptions
Currency: Indian Rupees (₹)
Current month fixed to April 2026
Seed data includes 30 transactions
Data spans January → April 2026
Role system is UI simulation only

In a real production app, authentication and backend APIs would manage roles.

✅ Requirement Checklist
Feature	Status
Summary Cards	✅
Trend Chart	✅
Donut Chart	✅
Transaction Table	✅
Search & Filtering	✅
Sorting	✅
Role-Based UI	✅
Insights Dashboard	✅
State Management	✅
Responsive Layout	✅
Empty State	✅
Dark Mode	✅
LocalStorage Persistence	✅
CSV Export	✅
Animations	✅
🎨 Design Philosophy
Aesthetic

Dark-first financial dashboard inspired by Bloomberg Terminal and modern SaaS apps.

Typography
DM Serif Display — Headlines
Instrument Sans — Body
DM Mono — Data & numbers
Color System
Neutral background
Gold highlight accent
Green = Income
Red = Expenses
Visualization

All charts are built using handcrafted SVG.

No external chart libraries.

Zero dependencies.

💡 Why This Project Matters

This project demonstrates:

Frontend architecture
Data visualization
State management
UX design
Performance optimization
Vanilla JavaScript mastery

A strong project for:

Frontend developer portfolio
Internship applications
SDE interviews
📦 How to Push to GitHub

Run the following commands:

git init
git add .
git commit -m "Initial commit - Ledger Finance Dashboard"
git branch -M main
git remote add origin https://github.com/yourusername/ledger-finance-dashboard.git
git push -u origin main
