# UPI and Digital Payment Transaction Trend Analysis

## Project Overview
This project analyzes sample UPI and digital payment transactions using Python. It demonstrates data inspection, exploratory data analysis, and chart generation.

> **Important:** The included dataset is synthetic and created for educational/demo use. It is not real bank, customer, or NPCI data. Findings describe only this sample and should not be presented as real-world market statistics.

## Repository Structure
```text
upi-digital-payment-analysis/
├── data/
│   ├── upi_digital_payment_raw_dataset.csv
│   └── upi_digital_payment_cleaned_dataset.csv
├── graphs/
│   ├── 01_monthly_transaction_trend.png
│   ├── 02_payment_method_count.png
│   ├── 03_transaction_value_by_method.png
│   ├── 04_transaction_status.png
│   ├── 05_state_wise_value.png
│   ├── 06_merchant_category_value.png
│   ├── 07_bank_wise_count.png
│   ├── 08_amount_distribution.png
│   ├── 09_hourly_transaction_trend.png
│   └── 10_average_amount_by_age_group.png
├── analysis.py
├── payment_analysis_summary.csv
├── requirements.txt
└── README.md
```

## Dataset Details
- **Raw dataset:** 1,225 rows and 13 columns. It includes intentionally introduced data-quality issues such as missing values, duplicates, inconsistent labels, invalid dates, and non-positive amounts.
- **Cleaned dataset:** 1,178 rows and 13 columns.
- **Main columns:** transaction ID, date, time, state, city, payment method, transaction type, merchant category, amount in INR, transaction status, device type, bank, and customer age group.

## Objectives
1. Analyze monthly transaction volume.
2. Compare transaction counts and transaction value by payment method.
3. Examine successful, failed, and pending transactions.
4. Compare state-wise and merchant-category transaction values.
5. Review bank-wise transaction counts.
6. Explore transaction amount distribution and activity by hour.
7. Compare average transaction amounts by customer age group.

## Visualizations

### 1. Monthly Transaction Trend
![Monthly trend](graphs/01_monthly_transaction_trend.png)

### 2. Transactions by Payment Method
![Payment method count](graphs/02_payment_method_count.png)

### 3. Total Transaction Value by Payment Method
![Transaction value](graphs/03_transaction_value_by_method.png)

### 4. Transaction Status Distribution
![Status distribution](graphs/04_transaction_status.png)

### 5. State-wise Transaction Value
![State-wise value](graphs/05_state_wise_value.png)

### 6. Merchant Category Transaction Value
![Merchant category](graphs/06_merchant_category_value.png)

### 7. Bank-wise Transaction Count
![Bank count](graphs/07_bank_wise_count.png)

### 8. Transaction Amount Distribution
![Amount distribution](graphs/08_amount_distribution.png)

### 9. Transactions by Hour
![Hourly trend](graphs/09_hourly_transaction_trend.png)

### 10. Average Amount by Age Group
![Age group](graphs/10_average_amount_by_age_group.png)

## How to Run

### 1. Clone the repository
```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Generate charts and summary
```bash
python analysis.py
```

The script reads the cleaned CSV in `data/`, regenerates the PNG charts in `graphs/`, and writes `payment_analysis_summary.csv`.

## Tools
- Python
- Pandas
- Matplotlib

## Limitations
- The data is synthetic and not representative of actual payment activity.
- Visual patterns are descriptive only and do not establish causation.
- Real payment trends should be analyzed with verified, appropriately licensed data.

## License
Educational/demo project. Add a license file if you plan to publish or redistribute it under specific terms.
