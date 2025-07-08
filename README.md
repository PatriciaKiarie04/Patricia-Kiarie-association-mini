# Market Basket Analysis with Association Rules

##  Project Overview

This project demonstrates market basket analysis using the Apriori algorithm to discover association rules in retail transaction data. The analysis reveals which products are frequently purchased together, enabling businesses to optimize:
- Product placement
- Promotional strategies
- Inventory management

##  Dataset Characteristics

- **Unique product selection** (no eggs/milk/bread):
  - Coffee, Protein Bars, Frozen Pizza
  - Red Wine, Dark Chocolate
  - Pet Food, Laundry Detergent
  - Fresh Flowers, Batteries, Vitamins, Ice Cream
- **20 simulated transactions** (2-5 items each)
- **Real-world retail patterns**:
  - Complementary products (wine + chocolate)
  - Household essentials bundles
  - Health/wellness combinations

##  Key Findings

### Top Association Rules

| Antecedents                  | Consequents       | Confidence | Support |
|------------------------------|-------------------|------------|---------|
| Red Wine, Frozen Pizza       | Dark Chocolate    | 83%        | 30%     |
| Laundry Detergent, Batteries | Toilet Paper      | 80%        | 25%     |
| Vitamins, Coffee             | Protein Bars      | 75%        | 25%     |

### Business Insights
1. **Wine & Chocolate Combo**  
   - 83% of customers who buy wine and pizza also buy chocolate  
   - *Action:* Create a "Movie Night Bundle" promotion

2. **Household Essentials**  
   - Detergent+batteries buyers are highly likely (80%) to need toilet paper  
   - *Action:* Place these in adjacent store aisles

3. **Morning Routine Items**  
   - Coffee and vitamin purchasers often buy protein bars  
   - *Action:* Cross-promote near checkout counters

##  Technical Implementation

### Dependencies
```bash
pip install pandas mlxtend