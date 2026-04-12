# **Individual Data Science Project**

## **INTRODUCTION**
This project was undertaken to investigate the kind of logistics that a company may apply to their customer data to finetune their marketing or improve their storefront. 

Research Questions:
* Are customers on mobile more likely to leave a review/longer review than web customers?
* Are certain subcategories more popular with specific age groups?

## **SELECTION OF DATA**
This dataset came from kaggle and represents the customer reviews of clothing for a ecommerce clothing business. The set includes appromximately 23000 records for women's clothing reviews. Key features used to answer the research questions were: Customer Age, Review Text, Channel, and Subcategory1.

For one question, entries with a null subcategory column ('Subcategory1') were dropped from the set. In the other, entries with a null Review Text column were dropped from the set.\
Data Preview:\
<img width="1128" height="225" alt="Screenshot 2026-03-25 at 3 10 57 PM" src="https://github.com/user-attachments/assets/294b4e04-73dd-43a4-8c7f-a695fb05a845" />


## **METHODS**
Data Manipulation Tools:
* NumPy, Pandas, SciPy

Data Visualization Tools:
* Seaborn, Matplotlib

Method:
* T-Test

## **RESULTS**
*Are customers on mobile more likely to leave a review/longer review than web customers?*

<img width="640" height="480" alt="ReviewLengthDistribution" src="https://github.com/user-attachments/assets/1cd865d6-b43a-4a87-b152-9951dca66508" />

The distribution of review length was nearly identical between the two channel types. This does not lend itself to any difference between the two groups in terms of behavior. The actual mean review length across platforms (308-309) is also intriguing as it is closer to the review character limit of 500 than expected. 

For further examintion, a two-tailed t-test with a confidence level of α = 0.05 was performed with the data. The null hypothesis is that the mean review length of web users was equal to the mean review length of the mobile users. The alternative hypothesis is that the mean review length of web users was not equal to the mean review length of mobile users. This can be represented using the format:

H<sub>0</sub>: 309.08214 = μ and H<sub>a</sub> : 309.08214 ≠ μ

After computing, the absolute value of the test statistic is 0.5363869120270773 and the critical value for the t-test is 1.9601451595523012. Since the test statistic is less than the critical value, the null hypothesis failed to be rejected. In ohter words, there is no evidence that there is a significant statistical difference between the mean mobile review length and the web mean review length. 

*Are certain subcategories more popular with specific age groups?*

<img width="547" height="481" alt="plot" src="https://github.com/user-attachments/assets/70c7c6eb-79b9-4a3b-b5ea-0e645a0249e6" />

The overall proportion of subcategories within all the reviews does not change significantly between age groups. While the exact percentage varies slightly, for example the 36-45 group having a slightly smaller than average portion of jackets while 65+ had a slightly higher portion, each of the age groups follow the same order in terms of how much of the total reviews that category had. This implies that there is no variance in popularity of a subcategory within the different age groups.  

## **DISCUSSION**

The lack of evidence to show a difference between review length for mobile and web users could suggest that the current UI in both formats are equally conducive to leaving a review. This is important to gauge because a frustrating UI to navigate could steer customers away from buying off the online shop. The mean length of the reviews itself being closer to the limit suggests that users are likely to leave a longer review. This factor may be important to businesses to consider since [as research has shown](https://openresearch.okstate.edu/server/api/core/bitstreams/05de9cd3-9bd9-4306-93f4-94dc00ac60bd/content#:~:text=Korfiatis%20et%20al.,and%20helpful%20for%20experience%20products.) , a longer review is helpful to potential customers. 

The lack in variance in which categories are popular with certain age groups is helpful to determining the kind of marketing the business would have to do. If the business was to put out personalized ads or develop a recommended purchases tool for their shop using customer data, they would not have to strongly consider age as a factor in choosing which products to promote. 

Further research may delve into the actual ratings given by customers and seeing if there are trends within the categories of clothing. There is also an interesting angle of finding common keywords used in the reviews and seeing if there's a correlation between the customer then recommending the product. 

## **SUMMARY**
This project applies company logistics to derive meaning from the statistical manipulation of customer data. The hypothesized variations between web users and mobile customers, as well as customers across different age groups, were failed to be supported by the data. 
