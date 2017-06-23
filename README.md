# Red-Wine-Data-Analysis-by-R

In this project, I will analyze the Red Wine Data and try to understand which variables are responsible for the quality of the wine. First I will try to get a feel of the variables on their own and then I will try to find out the correlation between them and the Wine Quality with other factors thrown in. Finally I will create a linear model to predict the outcome of a test set data.

# Table of Contents

1. redWineAnalysis.html - The Final project report.

2. redWineAnalysis.md - The viewable markdown file with plots and without codes.

3. redWineAnalysis.rmd - The viewable R markdown file with codes and without plots.

4. references.txt - List of references.

5. wineQualityReds.csv - The dataset from which analysis was done.

# Conclusion of the Analysis

In this data, my main struggle was to get a higher confidence level when predicting factors that are responsible for the production of different quality of wines especially the 'Good' and the 'Bad' ones. As the data was very centralized towards the 'Average' quality, my training set did not have enough data on the extreme edges to accurately build a model which can predict the quality of a wine given the other variables with lesser margin of error. So maybe in future, I can get a dataset about Red Wines with more complete information so that I can build my models more effectively.

Initially when I was writing and developing for this project, I saw that some wines didn't have citric acid at all. Also the others showed almost a rectangular distribution. My first thought was maybe this was bad data or incomplete data. But then I researched further about wines. I saw that citric acid actually is added to some wines to increase the acidity. So it's evident that some wines would not have Citric Acid at all. So actually this was in parallel to my experimental findings.

The other variables showed either a Positively skewed or a Normal Distribution.

First I plotted different variables against the quality to see Univariate relationships between them and then one by one I threw in one or more external factors to see if they together have any effect on the categorical variable. I saw that the factors which affected the quality of the wine the most were Alcohol percentage, Sulphate and Acid concentrations.

I tried to figure out the effect of each individual acid on the overall pH of the wine. Here I found out a very peculiar phenomenon where I saw that for volatile acids, the pH was increasing with acidity which was against everything I learned in my Science classes.

But then to my utter surprise, for the first time in my life as a data analyst, I saw the legendary Simpson's Paradox at play where one lurking variable was reversing the sign of the correlation and in turn totally changing the trend in the opposite direction.

In the final part of my analysis, I plotted multivariate plots to see if there were some interesting combinations of variables which together affected the overall quality of the wine. It was in this section I found out that density did not play a part in improving wine quality.

For future analysis, I would love to have a dataset, where apart from the wine quality, a rank is given for that particular wine by 5 different wine tasters as we know when we include the human element, our opinion changes on so many different factors. So by including the human element in my analysis, I would be able to put in that perspective and see a lot of unseen factors which might result in a better or worse wine quality. Having these factors included inside the dataset would result in a different insight altogether in my analysis.
