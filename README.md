# Decision-Trees-Will-an-online-shopper-make-a-purchase-
The objective is to predict whether a customer will make a purchase in a session.
In physical retailing, a salesperson can offer a range of customized alternatives to shoppers based on experience or customer behaviour. This has an important influence on the effective use of time, purchase conversion rates, and sales figures.
The dataset was formed so that each session would belong to a different user in a 1-year period to avoid any tendency to a specific campaign, special day, user profile, or period.
The objective is to predict whether a customer will make a purchase in this session. Every time a web page is served to the user, the online store will make a prediction of how likely it is that the customer will purchase. The store can use this probability to customize buying offers, provide discounts, offer purchase advice, etc.

Notes on Selected Features

(ADMINISTRATIVE, ADMINISTRATIVE_DURATION, INFORMATIONAL, INFORMATIONAL_DURATION, PRODUCT_RELATED, PRODUCT_RELATED_DURATION)
- These features represent the number of different types of pages visited by the visitor in that session and the total time spent in each of these page categories. The values of these features are derived from the URL information of the pages visited by the user and updated in real time when a user takes an action, e.g. moving from one page to another

(BOUNCE_RATE, EXIT_RATE, PAGE_VALUE)
- These features represent the metrics measured by "Google Analytics" for each page in the e- commerce site. The value of "Bounce Rate" feature for a web page refers to the percentage of visitors who enter the site from that page and then leave ("bounce") without triggering any other requests to the analytics server during that session. The value of "Exit Rate" feature for a specific web page is calculated as for all pageviews to the page, the percentage that were the last in the session. The "Page Value" feature represents the average value for a web page that a user visited before completing an e-commerce transaction.

(SPECIAL_DAY)
- This feature indicates the closeness of the site visiting time to a specific special day (e.g. Mother’s Day, Valentine's Day) in which the sessions are more likely to be finalized with transaction. The value of this attribute is determined by considering the dynamics of e- commerce such as the duration between the order date and delivery date. For example, for Valentine’s day, this value takes a nonzero value between February 2 and February 12, zero before and after this date unless it is close to another special day, and its maximum value of 1on February 8.

(OPERATINGSYSTEMS, BROWSER, REGION, TRAFFICTYPE, VISITORTYPE) 
- Attributes of specific user session
