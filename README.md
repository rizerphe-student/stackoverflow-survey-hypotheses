# Team Members

1. Bohdan Opyr
2. Radomyr Husiev
3. Roman Zaletskyy

# Objective of the Project

The objective of our research project is to conduct a thorough analysis of the data obtained from the [Stack Overflow Developer Survey](https://insights.stackoverflow.com/survey). This comprehensive dataset comprises a wealth of information regarding the demographics, professional practices, and technological preferences of developers. Our analysis will primarily concentrate on the interrelations between various programming languages as reported by the survey participants.

# Description of the Dataset

Our analytical focus will be on the dataset’s provision about the current and projected usage of specific programming languages by the respondents. Essential variables have been earmarked for detailed examination, as outlined below:


*In the dataset we have two variables that are relevant to our analysis:*

- `1` or `0` for each language - whether the respondent used the language last year or not
- `1` or `0` for each language - whether the respondent would like to use the language in the next year or not

*From the dataset we can also find variables*:

- `1` or `0` for each language - whether the respondent is inclined to use the language or not given that they used R last year
- `1` or `0` for each language - whether the respondent is inclined to use the language or not given that they used R last year and desire to continue using R in the next year

# What we want to test

1. **Correlation between the use of R and the inclination to use Python in the forthcoming year:**
    - Null Hypothesis (H0): The average inclination to use Python in the next year among R users is equal to the average inclination to use Python in the next year among the whole sample.
    - Alternative Hypothesis (H1): The average inclination to use Python in the next year among R users is greater than the average inclination to use Python in the next year among the whole sample.
    - We will use the z-test to make a decision whether to reject the null hypothesis or not. The z-test is appropriate for our analysis because the sample size is large enough (n > 30) and the population standard deviation is known.

2. **Correlation between the desire to use R in the forthcoming year and the desire to use Python in the same time frame:**
    - Null Hypothesis (H0): The average inclination to use Python in the next year among individuals who are using and desire to use R in the next year is equal to the average inclination to use Python in the next year among the general population.
    - Alternative Hypothesis (H1): The average inclination to use Python in the next year among individuals who are using and desire to use R in the next year is lower than the average inclination to use Python in the next year among the general population.
    - We will use the z-test to make a decision whether to reject the null hypothesis or not. The z-test is appropriate for our analysis because the sample size is large enough (n > 30) and the population standard deviation is known.

3. **Linear correlation between age and the wish to persist in using R:**
    - Null Hypothesis (H0): There is no linear relationship between a respondent's age and their desire to continue using R among the current R-using population.
    - Alternative Hypothesis (H1): There is a positive linear relationship between a respondent's age and their desire to continue using R among the current R-using population.
    - Regression Analysis: We will conduct a linear regression analysis to test these hypotheses, using age as the independent variable and the desire to continue using R as the dependent variable.

# Initial Observations

- The bulk of the survey responses intended for our analysis originates from the United States and Germany, indicating a potential regional bias that warrants consideration in the context of broader applicability.
- R has been employed by 4% of survey participants, while its utilization by professional developers lies marginally lower at 3%.
- Conversely, 5% of individuals in the process of learning to code reported R usage this year, casting doubt on the straightforwardness of our hypothesis regarding age and continuing R use, and signaling the need for deeper scrutiny.
- A significant 49% of respondents acknowledged utilizing Python this year, suggesting its widespread adoption.
- The survey boasts a robust sample size with 89,000 responses, thereby affording a strong foundation for substantive research conclusions.
- Initial data indicates that a mere 39% of R users exhibit a preference for its continued application, in stark contrast to Python where this figure escalates to 66%. This initial disproportionality must be taken into account when juxtaposing findings against the general survey backdrop.
