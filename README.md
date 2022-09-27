# Bakery-Performance-Evaluation

This problem aims at evaluating the performance of a bakery chain so far and providing insights into which promotional offers worked best for them and understand their clients' preferences. To increase sales, the restaurant regularly offers a variety of promotions. This reminds customers of the brand and motivates them
to dine with them more frequently. However, customer preferences and dining patterns differ. Thus, determining which offer to send and which channel to
send it with can be a complex task, since it’s not obvious when a customer will be receptive to a given offer. If too many irrelevant promotions are sent to the user, they will become annoyed and turn off the functionality and/or lose affinity for the brand.
A promotion is delivered to each customer on Sundays. It expires in when the new offer is received. With each time window, the customer can:
1. Make no purchases
2. Make a purchase with the promotion
3. Make a purchase without the promotion
The goal is to drive the customer to make a purchase.

For every customer, for every week, we have a record in this table.
![image](https://user-images.githubusercontent.com/113396912/192403002-1a795e37-f666-4209-b4c3-b38eeca92e42.png)

-> Purchase - boolean indicating whether they made at least one purchase in the time period the offer was active
-> TotalSpend - total amount the customer spent for the last order
-> CouponUsed - boolean indicating whether the coupon was used in that time period

Purchases made using a coupon suggest that the customer is aware of the brand and attracted to it. However, it is noticed many customers either unsubscribing to the offers or making purchases without the coupons. This indicates that the reward was not attractive to the customer or the channel did not attract the customer’s attention. The bakery believes that by changing one or both of these, they could have enticed the customer into taking the reward.

In this project, we are trying to understand correlations to coupon usage. I have tried to analyse:
1. The inputs that matter to predict whether a coupon will be used.
2. The best ways of representing the data. 

Data retrieval, cleaning and organizing has been performed using Pandas. Exploratory Data Analysis has been carried out with the help of heat maps and other graphs which highlight the most important features and depict a visual comparison between them. Trends and patterns have been presented using various charts in Matplotlib and Seaborn.

The scope of this project can be extended by training a model with these features to forecast future sales and coupon usage patterns. 
