# Mod3Kickstarter
Analysis of Kickstarter campaign success

Files:
- Analysis.ipynb: Loading,cleaning,modeling of data
- Kickstarter_data: Folder with all the .csv files used in the analysis
- Visualizations: Folder with some visualizations of the data

Overview:
You have an idea and want to start a Kickstarter campaign to raise money in order to make your idea a reality. You’re not sure though because you don’t want it to end in failure.
In this project, I aim to see if we can determine factors that play an important role in determining the success of a Kickstarter campaign to get an idea before someone launches the campaign.

Big Questions:
- What kind of trends are there with regards to success of campaigns?
- What are the most important factors in the success of campaign?
- What might these factors imply?

Models Used:
- Random Forest
- XGBoost

Findings:
Feature Importance By weight:
- When campaign started and ended
- How much they were trying to raise
- Length/duration in top 10
Feature Importance By Gain:
- Splitting on Year launched gave a lot of gain
- Mostly Categories in the top 10
- Length also in top 10

Conclusions:
- Length of Campaigns definitely plays a big role, it was an important feature in both how many times it was used in the trees as well as giving a good amount of information gain
- Category or the type of the campaign also has an impact on giving information gain, makes sense as was seen in the earlier bar graph, certain categories did much better than others
- Starting/end date and the year the campaign was launched were important features, but not good for future predictions due to variability

Next Steps:
- Remove certain features that don’t help with future predictions
  - Start/end date, launch/end year
  - Staff pick may not be useful to predict, but may be something to aim for when starting a campaign
- Make predictions on campaigns that are currently live and see how accurate they are once completed


