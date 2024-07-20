**CUT-OFF GRADE OPTIMIZATION USING MACHINE LEARNING ALGORITHMS (LINEAR REGRESSION AND NEURAL NETWORK)**

In this project, a model was developed for a potential mining project with a production capacity of 500,000 tons.

![cog_opt](https://github.com/user-attachments/assets/53de02e7-792a-42c1-9731-9e253f5c1159)

Using ore tonnage and grade data, random selections were made, and the NPV (Net Present Value) was calculated based on the following variable parameters:

- Variable Mining Unit Costs: Mining unit costs are adjusted according to different mining capacities, reflecting economies of scale and potential cost increases.
- Yield Values: Yield values vary depending on the ore grade, accounting for different ore characteristics and processing efficiencies.
- Variable Processing Costs: Processing costs are adjusted based on the ore grade, reflecting variations in processing requirements and the cost per ton processed.
- Fluctuating Product Selling Prices: The project considers varying product selling prices to account for market volatility and price fluctuations.
- Variable Investment Costs: Investment costs are calculated for different plant capacities, reflecting the investment required for equipment, infrastructure, and other fixed assets.
- Loan Repayment: Loan repayment schedules are integrated for the plant investment, simulating the impact of debt financing on cash flow.

In the second phase, 10,000 simulations were performed for the 500,000-ton capacity, and the maximum, minimum, and average NPV values were determined through random selection.

![newplot (4)](https://github.com/user-attachments/assets/7630b863-92c6-4afd-b501-c5c9d4464dd6)

In the third phase, the Break-Even Grade value for each year was identified and extracted from the database.

For Cut-Off Grade Optimization, with the aim of maximizing NPV, future price values determined by DeepAR (https://github.com/3ayramkoc/AutoGluon) were used to investigate which grades should be produced in which years. The model targeted the maximization of NPV based on the discounted future price values. The R2 value was calculated for Linear Regression, and model training was conducted. The ore metal content was distributed under the discounted price curve, and the metal ratio within the 500,000 tons of ore was calculated for each year to determine the optimized grade value for production.

In the final stage, the NPV value was calculated for production using the optimized COG values. The maximum NPV determined from 10,000 iterations was 97 million USD, while the optimized NPV value reached 117 million USD.
