# **Individual Data Science Project**

## **INTRODUCTION**
This project was undertaken to investigate the kind of logistics that a company may apply to their customer data to finetune their marketing or improve products. 
Research Questions:
* Are customers on mobile more likely to leave a review/longer review than web customers?
* Are certain subcategories more popular with specific age groups?

## **SELECTION OF DATA**
This dataset came from kaggle and represents the customer reviews of clothing for a ecommerce clothing business. The set includes appromximately 23000 records for women's clothing reviews. For one question, entries with a null subcategory column ('Subcategory1') were dropped from the set. In the other, entries with a null review text section were dropped from the set.\
Data Preview:\
<img width="1128" height="225" alt="Screenshot 2026-03-25 at 3 10 57 PM" src="https://github.com/user-attachments/assets/294b4e04-73dd-43a4-8c7f-a695fb05a845" />


## **METHODS**
Tools:
* NumPy, Pandas, Matplotlib, Scikit

Methods:
* T-Test, Linear Regression

## **RESULTS**
What answer was found to the research questions; what did the study find?\
*Are customers on mobile more likely to leave a review/longer review than web customers?*

<img width="640" height="480" alt="ReviewLengthDistribution" src="https://github.com/user-attachments/assets/1cd865d6-b43a-4a87-b152-9951dca66508" />

The distribution of review length was nearly identical between the two channel types. This does not lend itself to any difference between the two groups in terms of behavior.

For further examintion, a two-tailed t-test was performed with the data. My null hypothesis being that the mean review length of web users was equal to the mean review length of the mobile users and my alternative hypothesis being that the mean review length of web users was not equal to the mean review length of mobile users. This can be represented using the format:

H<sub>0</sub>: 309.08214 = μ and H<sub>a</sub> : 309.08213 ≠ μ

*Are certain subcategories more popular with specific age groups?*
Was the tested hypothesis true?
## **DISCUSSION**
What might the answer imply and why does it matter?\
How does it fit in with what other researchers have found?\
What are the perspectives for future research?

## **SUMMARY**
