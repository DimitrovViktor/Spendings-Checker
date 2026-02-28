# Spendings-Checker

C# (.NET + Blazor) application which checks the user's spendings and monthly subscriptions and gives graphs, trends, and estimates of potential future purchases.

## Home Page

Account management system where each account has its own currency, date format, and CSV column mappings. Main currency and conversion rates are configurable at the top. Multiple CSV file uploads per account are supported, uploaded files are shown and can be deleted at any time. Selected files are previewed before uploading.

![Accounts](https://github.com/user-attachments/assets/da6afbce-e027-465e-b37b-062ebef36afa)

## Spendings Page

Transactions are taken from CSV files and listed along with total amounts of spendings, earnings, and the final change in balance. Sortable by date, company, or amount. Filterable by account when multiple accounts exist. Company names and payment processors are auto-detected from transaction descriptions.

![Spendings](https://github.com/user-attachments/assets/3a6ccc1a-3def-43e6-a23e-495ba1daa88d)

## Subscriptions Page

Transaction info is taken from CSV files and recurring payments are marked as subscriptions. Each company has a profile with details for all recurring payments. Companies are classified as active subscriptions, recurring returners, cancelled, one-off, or irregular based on charge frequency and amount consistency.

![Subscriptions](https://github.com/user-attachments/assets/aff81e7f-2310-40d4-8780-c993161a3c90)

![Subscriptions2](https://github.com/user-attachments/assets/8b3e60f3-1c4b-4abb-b285-6b66994cf60a)

## Projections Page

Predictions are displayed based on info from CSV files. Projections show how much money the user may spend in the future if they continue to spend in the same patterns. Three projection modes:

- **All Spendings** — linear trend across all transactions

- **Sub-Aware** — separates subscription charges from irregular spending, projects each independently

![Projections](https://github.com/user-attachments/assets/f3f4ed13-3f5e-4914-9938-324bb9c2d5fb)

Interval can be set to weeks, months, or years with configurable periods ahead. Companies can be toggled on/off and the chart shows a "without deselected" line to compare. Active subscriptions and recurring returners support cancellation date scheduling which excludes them from projections after that date.

## TO-DO:

- Subscription only projections
  
## Potential Future Work

- Planned spendings - add planned/scheduled purchases(e.g. user wants to buy something) to future estimations
