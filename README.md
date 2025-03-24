# Consumer Behaviour Analysis
I carried out an exploratory data analysis on this consumer dataset to uncover trends and insights, the processes include data cleaning, data processing and visualizations of my findings.
## Project Ojectives
An e-commerce store wans to carry out Exploratory Data Analysis on their past consmer data to uncover trends and patterns in the business.
## Dataset Used
<a href="https://github.com/blessingajidahun/Exploratory-Data-Analysis/blob/main/ecommerce_consumer_behavior_analysis_data.csv">Dataset</a>
## Processes
After downloading the dataset, the first thing I did was to go through it, familiarize myself with what each column meant, then I checked for duplicate values, there was none, I also checked for blank cells, there was none. This means the dataset is clean and I can go on with my analysis. I used pivot table majorly for this analysis and certain functions like CORREL and IF statements.
## Key Insights and Recommendations for each task
### TASK 1: Customer demographics and purchase behavior: you are to group the customer age into two groups young (below 35 years) and old (above 36) and compare which group spends more on products, which category each group patronizes more and their income level.
I created a new column named “age group”, then grouped the customer age into young and old using IF statement, then I used pivot table to carry out my analysis.

#### Key Insights Discovered:
Young Customers Spend More Than Older Customers
Older Customers Still Contribute Significantly
o	While younger customers spend more, older customers still have a substantial share (close to young customers).
o	This could indicate brand loyalty or a preference for quality over quantity in purchasing habits.
#### Top Spending Categories for Old vs. Young Customers
•	Old customers' highest spending categories:
- Jewelry & Accessories ($8,697)
-	Toys & Games ($8,217)
### View Dashboard Intercation
-Sports & Outdoors ($6,689)
•	Young customers' highest spending categories:
- Software & Apps ($8,061)
- Sports & Outdoors ($7,921)
- Groceries ($8,274)
•	Young customers seem to prioritize groceries, tech, and experiences, while older customers spend more on durable goods like jewelry and accessories.
•	Young Customers Dominate Both High and Middle Income Segments
- Younger customers have higher representation in both income levels, making them a key target for premium and mid-range product offerings.
•	Older Customers Have a Smaller Presence Across Income Segments
o	They are slightly behind younger customers in both high and middle-income brackets, indicating lower spending power or purchasing enthusiasm in certain categories.
#### Recommendations:
1.	Target Younger Customers with Promotions & Personalized Offers
o	Since they spend more, use discounts, flash sales, or loyalty rewards to increase retention.
2.	Focus on online grocery delivery, tech accessories, and fitness products for younger customers,  while for older customers, focus more on durable goods like jewelry and accessories.

### TASK 2: Customer loyalty and retention analysis: how often do customers return purchased items from the store, how customer satisfaction affects brand loyalty.
I used pivot table to find the average return_ rate and CORELL function to analyze the correlation between customer satisfaction and brand loyalty.
#### KEY INSIGHTS
An overall average return rate of 0.954 (which is close to 1) means that customers return almost every product they purchase on average. This is a very high return rate and could indicate serious business challenges.
Correlation of customer satisfaction to brand loyalty is -0.03458. This means there is no correlation between customer satisfaction and brand loyalty.
#### RECOMMENDATIONS
Product Quality Issues
- Customers might be dissatisfied with the quality of the products they receive, leading to frequent returns. However, further analysis (which will be explained later) reveals that products high customer satisfaction ratings were also returned, product quality may not be the reason for high return rate.
- There could be mismatch between product descriptions(images, sizes, specifications) and reality, improve product listings with clearer descriptions and real customer reviews.
- Review return policies to balance flexibility with business sustainability if the store offers easy or free returns of purchased products.
#### TASK 3: Pricing and discounts effectiveness: do discount sensitive customers spend more when products are discounted, how does the discount used affect return rate, are customers with high income interested in discounts.
I used Pivot table to analyze customer’s discount sensitivity and their spending behavior, likewise I used Pivot table to analyze the effect of discount used on return rate.
#### Key Insights Discovered: 
- Total Purchase Amount (Sum of Purchase_Amount)
  -	Not Sensitive customers spent $88,536 in total.
  -	Somewhat Sensitive customers spent $90,001 in total.
  -	Very Sensitive customers spent $96,526 in total.
- Customer Count (Count of Customer_ID)
  -	Not Sensitive: 331 customers
  - Somewhat Sensitive: 319 customers
  - Very Sensitive: 350 customers
  - The Very Sensitive group has the highest number of customers (350), meaning discounts attract more buyers.
- However, the Not Sensitive group also has a significant presence (331 customers), showing that many customers buy without discounts.
- The Very Sensitive group (those who frequently use discounts) spent the most in total, suggesting that discounts help drive overall sales.
- However, the difference in total spending among groups is not drastic, meaning non-sensitive customers still contribute significantly.
- Running discounts could be effective in increasing customer volume, even if it doesn’t drastically raise individual purchase amounts. 
- Effect of discount on return rate
  - More returns came from discounted purchases (521) than non-discounted purchases (479).
  - Implication: Customers who used discounts returned more items than those who paid full price, this suggests that discounts may encourage impulse buying, leading to more returns.
- Income level and discount usage
  - High-income customers used discounts slightly more (515) than middle-income customers (485).
  - Implication: Contrary to the common assumption that only lower-income customers seek discounts, high-income earners also take advantage of discounts.
  - The difference (515 vs. 485) is not very large, suggesting both income groups actively use discounts. In a nutshell, discount appeals to all income level

### TASK 4: Purchase behavior and preferences: how does the purchase category affect shipping preference (are customers that purchase a particular product likely to use a particular mode of shipping), what are the peak shopping hours and days of the week?
### KEY INSIGHTS DISCOVERED:
- High Express Shipping Demand:
  - Office Supplies (18), Gardening & Outdoors (18), Health Supplements (15), Home Appliances (14), Jewelry & Accessories (14), Baby Products (14)
  - Customers purchasing these items likely need fast delivery (e.g., urgent needs or perishable items like health supplements).
- High Standard Shipping Usage:
  - Home Appliances (20), Animal Feed (19), Jewelry & Accessories (19), Books (16), Electronics (17), Clothing (13)
  - These items may be less time-sensitive or bulkier, making standard shipping more suitable.
- Categories with No Strong Preference:
  - Food & Beverages, Sports & Outdoors, Packages, Software & Apps, Toys & Games
  - Customers in these categories seem flexible with shipping options, meaning price or promotions may influence their choice.
#### Recommendations	
- Promote express delivery discounts for Office Supplies, Gardening & Outdoors, and Health Supplements since these categories have higher express demand.
- Encourage bulk or planned purchases by offering discounted standard shipping on Home Appliances, Electronics, and Animal Feed.

### TASK 5: Marketing and ad engagement: does social media’s influence affect the purchase amount, does social media influence affect product rating.
I used Pivot table to carry out this analysis.
#### Key Insights Discovered:
- Higher Social Media Influence = Higher Purchase Amount
  - Customers with high social media influence spend the most (Avg. Purchase Amount = $284).
  - Customers with no social media influence spend the least ($263).
  - This suggests that social media plays a positive role in encouraging spending.
- Medium Influence Group Also Spends More
  - Even customers with medium influence ($280.12) spend more than those with low influence ($272.50), reinforcing the impact of social media engagement.
- Customers with High Social Media Influence Give More Ratings
  - The highest number of product ratings (268) comes from customers with high social media influence.
  - This suggests that socially engaged customers are more likely to leave reviews, possibly due to exposure to brand content and engagement with online communities.
- Customers with No Social Media Influence Still Leave Many Ratings
  - The "None" group (247 ratings) is close to the "Low" (249 ratings) and "Medium" (236 ratings) groups.
  - This suggests that even customers who are not active on social media still leave reviews, possibly due to other forms of engagement (e.g., emails, website prompts).
- Medium Influence Customers Give the Least Ratings
  - Customers with medium social media influence give the fewest product ratings (236).
  - This could indicate that casual social media users are not as motivated to leave reviews compared to highly engaged or non-social media users.
#### RECOMMENDATIONS:
- Since social media-influenced customers spend more, we  increase efforts in targeted ads, influencer collaborations, and content marketing to engage customers.
- We can turn the “none social media influenced category into engage followers by running social media campaigns and offer exclusive discounts to encourage engagement.
- Since highly influenced customers are already reviewing, we should amplify this with campaigns like:"Share your review and get a discount!", "Post your purchase and tag us to win rewards!"
### TASK 6: Return rate and product quality: do product with low rating have higher return rates, which product category has the highest return rate, are dissatisfied customers more likely to return products
I used pivot table to carry out this analysis.
### Key Insights Discovered:
- Higher-Rated Products (4 & 5) Have the Most Returns:
  - Rating 5 has the highest total returns (211), followed by rating 4 (210).
  - Despite being high-rated, these products see substantial returns, likely due to unmet high expectations or buyer’s remorse.
- Lower-Rated Products (1 & 2) Have a Moderate Return Rate:
  - Rating 1 (205 total returns) and Rating 2 (189) suggest that low-quality products also face returns, but not as much as high-rated ones.
  - This could indicate that customers expect issues with low-rated products and may hesitate to return them.
- Return Rate Increases with Product Rating (1 → 5):
  - Lower-rated products (1, 2, 3) have fewer returns in category 2 (frequent returners).
  - Higher-rated products (4 & 5) have the most category 2 returns (72 & 63), meaning customers return them multiple times.
- Higher Overall Returns for High-Rated Products (4 & 5):
  - Rating 5 has the highest total returns (211), followed by rating 4 (210).
  - Despite high quality, these products are still returned often—possibly due to high expectations.
- These discoveries made me do a further research and analysis on the purchase intent, to know possible reasons why high rated products are returned. The following insights were what discovered:
- Impulsive and Wants-Based Purchases Drive Returns for Low-Rated Products:
  - Product Rating 1 has the highest wants-based return rate (59).
  - Impulsive returns are also highest for rating 4 (65), suggesting some customers regret impulsive high-quality purchases.
  - Need-Based Purchases Have the Highest Returns for Mid-Rated Products:
  - Product Rating 2 has the highest need-based returns (63), implying that essential products with mid-level quality don’t fully satisfy users.
- Planned Purchases Have the Lowest Return Volatility:
  - Return rates for planned purchases remain stable across all ratings (43-59).
  - This suggests planned buyers make more informed and satisfactory decisions.
- The Top 3 returned product categories are:
  - Electronics with 54 counts of return rate, Sports & Outdoor – 51 counts of return rate and finally Jewelry & Accessories and Home Appliances categories have 50 counts pf return rate each.
- Dissastisfied customers are more likely to return products. The analysis showed that Not Satisfied customers have a counts of 610 return rate, while Satisfied customers have a count of 390 return rate.
#### Recommendations
  - Enhance product durability, usability, or packaging to reduce dissatisfaction-driven returns
  - Offer extended warranties or trials to build customer confidence
  - Since these essential products have high returns, focus on better materials, packaging, and durability.
  - To discourage impulse returns, implement a restocking fee or provide returns as store credit instead of cash refunds

- Dashboard Interaction <a href="https://github.com/blessingajidahun/Exploratory-Data-Analysis/blob/main/Image.PNG">View dashboard</a>

### Dashbaord
![Image](https://github.com/user-attachments/assets/ba1f5577-474c-4f7f-aed2-4300e71312fc)


