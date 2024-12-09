# Swire-Coca-Cola-Capstone

## Summary of Business Problem
Swire Coca-Cola operates six facilities that produce approximately 192 million cases of beverages annually. However, the plants experience a production shortfall, producing only 94.4% of the total intended cases due to unplanned mechanical breakdowns and maintenance issues. This gap, costing the company approximately $60 million in lost productivity annually, results from unanticipated downtimes caused by machinery failures across various production lines. The current process relies on reactive maintenance through an Internal Warehouse Controller (IWC) system, which issues work orders only after machinery failures occur, leading to significant delays in repairs and downtime.

## The Group Solution to the Problem
In order to predict machinery downtimes in the factories, we created a survival analysis model. This was used as the dependent variable (machine downtime) is continuous and time determined. Survival analysis creates a visualization for probability of failure for each individual equipment ID, which provides the benefit of doing routine replacement/check up in these areas before the machine is likely to fail.

## My Contribution
One of the primary issues with tackling a highly dimensional dataset is finding how best to break the information down into more digestible pieces. I was interested in finding what features in the dataset had the best sectionality to determine downtime. I discovered that there were two types of workorders for machine downtime being reported, predicted and unpredicted. Upon further research, I found that unpredicted machine failures occur much more often and lead to higher downtimes on average. Thus, targetting these types of workorders would be highly beneficial, and could be quickly implemented by having routine maintainence on the highest machine type failures. We focused on the machine types unpredicted failures for our final survival analysis modeling that we presented to the Swire Coca-Cola Team.

## The Business Value of the Solution
A predictive maintenance solution would allow Swire Coca-Cola to anticipate and mitigate these downtimes. By predicting when and why machinery failures are likely to occur, the company can schedule proactive maintenance, reduce unplanned downtimes, increase production efficiency, and save millions annually. In addition, such a system would help Swire Coca-Cola maintain optimal production levels to meet demand and reduce maintenance costs by ensuring parts are stocked in advance.

## Difficulties Along the Way
A significant difficulty in this project was the lack of available data. We were hoping to predict downtime for individual equipment IDs, however 80% of the information was missing from the dataset. We could fortunately use another variable that offered a more broad focus on which machines were failing, but this was an opportunity to experience the difficulties of working with real world data. 

Later on when we were creating the survival analysis model, our output was only visualizing when the likelihood of failure was 100% instead of the expected downward slope. After ruling out some of the potential issues, we discovered that the data being input to the model was an average fail time of each machine part instead of the raw fail times.

## What We Learned
Working with real world data presents a number of challenges, primarily related to data cleaning and dimensionality. We quickly realized the importance of spending lots of time at the beginning to clean and do exploratory data analysis would help us in the long run. Having workable data and a deeper understanding of the dataset made our analysis in the end much easier and more insightful. 
