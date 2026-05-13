# **Amazon Sales Performance & Exploratory Data Analysis (EDA)**

### ****Project Overview****
This project performs an in-depth Exploratory Data Analysis (EDA) on an Amazon sales dataset containing 50,000+ transaction records. The primary objective of this analysis is to uncover actionable business insights regarding revenue generation, customer demographics, product performance, and seasonal sales trends.

By transforming raw transaction data into visual dashboards, this project highlights key areas where marketing, inventory, and customer retention strategies can be optimized.

### ****Dataset Details****
The dataset (amazon.csv) consists of 50,000 rows and 13 columns, representing individual customer orders.

### ****Key Features Include**** 
********order_id & order_date:******** Unique transaction identifiers and timestamps.

********product_category & product_id:******** Item details and classifications.

********price, discount_percent, discounted_price:******** Pricing metrics.

********quantity_sold & total_revenue:******** Sales volume and gross revenue.

********customer_region & payment_method:******** Geographic and transactional preferences.

********rating & review_count********: Customer satisfaction metrics.

### ****Key Business Insights****
Based on the data visualizations generated in this analysis, several key trends were identified:

****1. Payment Preferences****
   
****Insight:**** [Top Payment Method] is the most trusted and utilized payment option among customers, handling [X%] of all order volume.

****Actionable Recommendation:**** Ensure checkout pipelines for [Top Payment Method] remain highly optimized. Consider strategic partnerships or cashback incentives to promote underutilized platforms.

****2. Revenue by Product Category****
   
****Insight:**** The [Top Category] category is the primary cash cow, driving [$X] in total revenue, significantly outperforming bottom-tier categories like [Lowest Category].

****Actionable Recommendation:**** Reallocate marketing spend to capitalize on the high demand for [Top Category], while conducting pricing and visibility audits for lagging categories.

****3. Monthly Sales Trends (Seasonality)****
   
****Insight:**** Sales volume is highly seasonal, with sharp revenue spikes in [Peak Month], followed by a noticeable slump during [Lowest Month].

****Actionable Recommendation:**** Scale up supply chain and inventory logistics prior to [Peak Month] to prevent stockouts. Implement off-season discount campaigns during [Lowest Month] to stimulate stagnant demand.

****4. Regional Market Share****
   
****Insight:**** [Top Region] dominates global sales, accounting for [X%] of total revenue. Regions such as [Lowest Region] hold only a [Y%] share, representing untapped growth potential.

****Actionable Recommendation:**** Double down on loyalty programs in [Top Region] to protect market share, and launch localized, aggressive promotional campaigns to penetrate [Lowest Region].

****5. Product Quality & Customer Satisfaction****
   
****Insight:**** [Top Rated Category] achieves the highest customer satisfaction with an average rating of [X.X]/5.0. However, [Lowest Rated Category] suffers from a low average rating of [Y.Y]/5.0.

****Actionable Recommendation:**** Flag the [Lowest Rated Category] items for immediate quality assurance reviews. High return rates and poor reviews in this segment could negatively impact overall brand trust.

### ****Technologies Used****
********Data Manipulation:******** pandas, numpy

********Data Visualization:******** matplotlib.pyplot, seaborn

********Environment:******** Jupyter Notebook
