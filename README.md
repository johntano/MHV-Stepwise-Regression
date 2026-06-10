## Explanatory Analysis using Stepwise Regression (A Case Study on My HealtheVet Customer Satisfaction)
### Overview
The VA's patient portal site, My HealtheVet (MHV), offers veterans 24/7 access to anything related to the healthcare they receive from the VA. During their time on the site, a random sample of users are asked to complete a short survey about their experience. We take this feedback and report to our customer any interesting findings to measure the success of MHV while identifying potential risks or opportunities.

The survey is distributed by ForeSee, a third-party vendor. The survey questions can be organized into six site elements: Satisfaction, Look & Feel, Navigation, Site Information, Site Performance, & Task Process. The survey has three questions for each site element where users grade specific parts of their experience with a scale from 1 to 10. ForeSee uses these responses to calculate a composite score for each site element to summarize the data (the calculation itself is proprietary information, so we do not have access to really know how these composite scores are generated). For our customer, the composite satisfaction score is the most important metric regarding survey feedback. At this time, this is an outdated survey and ForeSee no longer acts as the survey vendor.

### Problem

The questions that make up the satisfaction score are too vague, as it generally asks users if the site meets their standards or if they are 'satisfied' with their experience. Although these are important questions to ask, it is difficult to determine what actions management needs to take as the language of the questions are too broad. We want to analyze if there is a significant relationship between the composite satisfaction score to the other questions in the survey. Once we find these relationships, we can find the most influential survey questions and determine which site elements should management prioritize.

### Key Findings

Here are the questions in the MHV survey that have the largest impact on satisfaction scores starting from the most significant (a unit increase in these questions also increase satisfaction scores):

• Please rate the procedures to accomplish tasks on this site.
• Please rate how well the site’s information provides answers to your questions.
• Please rate how well the site layout helps you find what you need.
• Please rate the time it takes to complete task(s) on this site.
• Please rate the thoroughness of information provided on this site.

### Conclusion

This analysis used stepwise regression to identify the survey questions that are the strongest predictors of overall user satisfaction. By reducing a large set of survey responses to a smaller group of high-impact drivers, the analysis provides a focused view of the aspects of the user experience that matter most to customers.

The results enable stakeholders to prioritize improvements based on factors that have the greatest influence on satisfaction rather than relying on intuition alone. Product teams can use these findings to direct resources toward enhancements that are most likely to improve the overall user experience and increase customer satisfaction.

Additionally, the identified drivers can serve as key performance indicators for future product evaluations, helping teams monitor whether new features and initiatives are improving the areas that users value most. By establishing a data-driven framework for prioritization, this analysis supports more informed decision-making and helps ensure that product investments are aligned with user needs and expectations.

Ultimately, the project demonstrates how statistical modeling can transform survey feedback into actionable insights, enabling the organization to better understand customer priorities, measure the impact of product changes, and continuously improve the user experience.

### Tools Used
• Python
• pandas
• numpy
• statsmodels
• Google Colab
