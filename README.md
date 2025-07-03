# Sales and Customer Behaviour
![image](https://github.com/user-attachments/assets/19e30abb-e0b7-4754-b3fb-7bced89a6c54)

🛒 An operational analytics project focused on customer basket size, purchase frequency, and return behaviours. Delivered via BigQuery SQL and designed to power data-informed commercial and customer retention decisions.

🎯 Project Objective
<br>To investigate purchasing patterns, basket composition, and customer return ratios — identifying value segments, potential risks, and actionable insights for merchandising, loyalty, and refund policies.

📈 Overview
<br>This project analyses millions of transaction and item-level records using SQL on Google BigQuery. The insights inform how customers purchase (basket size and channel), when they return (by rate and timing), and who might require closer monitoring based on refund risk or purchasing behaviours.

📊 Key Metrics Explored
- Basket size and composition by user and transaction
- Average Order Value (AOV) by basket band (e.g. single item vs 10+ items)
- Purchase frequency and customer lifespan
- Weekend vs weekday buying patterns
- Return rate percentage and days to return
- Return risk tiers (e.g. 30%, 60%, 90%+)

🧠 SQL Highlights
- Join logic between transactions, transactionsanditems, and product_returns
- CASE statements to bin basket size and return ratios
- Use of DATE_DIFF, EXTRACT(DAYOFWEEK), and nested aggregations
- Filters to identify customers with more than 50 returns
- Use of HAVING for risk flagging (e.g. return rate > 30% AND < 7 days)

📦 Basket Insights
- Users buying 5+ or 10+ items tend to have higher AOV — suggesting bundling opportunities.
- Weekend vs weekday patterns highlight volume surges on weekends, offering scheduling tips for fulfilment.
- Single-item baskets dominate, but contribute less total value than multi-item orders.

⚠️ Return Risk Profiling
Return analysis includes:
- Return ratio per customer and corresponding value of returned orders
- Time to return — with flags for customers returning within 7 days
- Return risk bins: customers with 30%+, 60%+, 90%+ ratios are isolated for operational review


📌 Next Steps
- Integrate product-level data to explore size/fit issues
- Overlay promotional activity to correlate with return surges


