# CouponRecommedation
🛒 Coupon Recommendation System
📌 Overview

This project implements a Market Basket Analysis system to recommend personalized coupons to customers.
Using association rule mining (Apriori algorithm), the system analyzes past purchase history and suggests the most relevant coupons before checkout.

⚙️ Features

Frequent Itemset Mining using Apriori.

Association Rules Generation with confidence & lift metrics.

Coupon Recommendation for customers based on transaction history.

Flask API Integration (via flask-ngrok) to serve recommendations.

Visualization Support using Matplotlib for rule analysis.

🛠️ Tech Stack

Python

Pandas, NumPy (data preprocessing)

mlxtend (Apriori & association rules)

Matplotlib (visualization)
🚀 How It Works

Load dataset containing customer transactions.

Transform data into basket format for Apriori.

Run Apriori to generate frequent itemsets.

Extract association rules based on support, confidence, and lift.

Recommend coupons:

If a customer has bought items A & B → Suggest item C coupon.

🔑 Key Functions

suggest_pre_cart_for_customer(customer_history, current_items)
→ Suggests coupons before checkout.

recommend_coupons(transaction)
→ Recommends coupons during a transaction.

📊 Example Output

Input: Customer has purchased [milk, bread]

Output: System suggests coupon for butter (based on strong association).

📈 Future Scope

Integrate with real-world e-commerce dataset.

Improve recommendations with hybrid ML models (Collaborative + Association rules).

Deploy as a REST API / Web App for live use.
