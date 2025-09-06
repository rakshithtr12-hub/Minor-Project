# Investigating the Role of AI-based Personalization in Shaping E-commerce Consumer Buying Behavior  

## 📌 Project Overview  
This project explores how **AI-based personalization** influences consumer buying behavior in e-commerce. Personalization has become one of the most effective tools for online retailers to drive engagement, improve customer loyalty, and increase sales.  

The project is part of my **MBA in Data Science** coursework (Amity University, 2025) and demonstrates how basic **data analysis** and **visualization** can highlight personalization trends.  

---

## 🎯 Objectives  
- Understand how personalization impacts consumer decisions.  
- Explore commonly used personalization tools in e-commerce.  
- Review real-world practices from companies like **Amazon, Netflix, Alibaba**.  
- Demonstrate simple **Python-based analysis** using mock data.  
- Discuss challenges like **privacy** and **ethical concerns**.  

---

## 📚 Literature Insights  
- McKinsey (2022): Personalization can increase customer satisfaction by **20%**.  
- Salesforce (2023): **80%** of customers prefer personalized experiences.  
- Amazon: Around **35% of sales** come from recommendations.  
- Netflix: Personalization is key for **retention and engagement**.  

---

## 🔎 Methodology  
- **Approach**: Qualitative + beginner-level analysis  
- **Data Source**: Secondary research (reports, blogs, company case studies)  
- **Tools**: Python (Pandas, Matplotlib)  
- **Focus**: Impact of personalization on sales & customer loyalty  

---

## ⚙️ Personalization Techniques Studied  
- Product **Recommendation Engines**  
- Personalized **emails & offers**  
- **Dynamic pricing** strategies  
- **Chatbots** and customer interaction tools  

---

## 🌍 Case Examples  
- **Amazon**: Recommendations account for ~35% of sales.  
- **Netflix**: Personalization improves user retention significantly.  
- **Alibaba**: Personalized layouts and real-time suggestions boost conversions.  

---

## 📊 Beginner-Level Python Example  

```python
import pandas as pd
import matplotlib.pyplot as plt

# Simulated product purchase data
data = {
    'Product': ['Product 1', 'Product 2', 'Product 3', 'Product 4', 'Product 5'],
    'User A': [1, 0, 1, 0, 1],
    'User B': [0, 1, 1, 0, 1],
    'User C': [1, 1, 0, 1, 0],
    'User D': [0, 1, 0, 1, 1]
}

df = pd.DataFrame(data)

# Count total purchases per product
df['Total Purchases'] = df.drop('Product', axis=1).sum(axis=1)

# Plot bar chart of product popularity
plt.figure(figsize=(6,4))
plt.bar(df['Product'], df['Total Purchases'], color='skyblue')
plt.title("Total Purchases per Product")
plt.xlabel("Products")
plt.ylabel("Number of Purchases")
plt.show()
