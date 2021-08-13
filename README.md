# Decision-Trees-Will-an-online-shopper-make-a-purchase-
The objective is to predict whether a customer will make a purchase in a session.
In physical retailing, a salesperson can offer a range of customized alternatives to shoppers based on experience or customer behaviour. This has an important influence on the effective use of time, purchase conversion rates, and sales figures.
The dataset was formed so that each session would belong to a different user in a 1-year period to avoid any tendency to a specific campaign, special day, user profile, or period.
The objective is to predict whether a customer will make a purchase in this session. Every time a web page is served to the user, the online store will make a prediction of how likely it is that the customer will purchase. The store can use this probability to customize buying offers, provide discounts, offer purchase advice, etc.

Feature Description

- ADMINISTRATIVE - Number of pages visited by the visitor about account management
- ADMINISTRATIVE_DURATION - Total amount of time (in seconds) spent by the visitor on account management related pages
- INFORMATIONAL - Number of pages visited by the visitor about Web site, communication and address information of the shopping site
- INFORMATIONAL_DURATION - Total amount of time (in seconds) spent by the visitor on informational pages
- PRODUCT_RELATED - Number of pages visited by visitor about product related pages
- PRODUCT_RELATED_DURATION - Total amount of time (in seconds) spent by the visitor on product related pages
- BOUNCE_RATE - Average bounce rate value of the pages visited by the visitor
- EXIT_RATE - Average exit rate value of the pages visited by the visitor
- PAGE_VALUE - Average page value of the pages visited by the visitor
- SPECIAL_DAY - Closeness of the site visiting time to a special day
- OPERATINGSYSTEMS - Operating system of the visitor
- BROWSER - Browser of the visitor
- REGION - Geographic region from which the session has been started by the visitor
- TRAFFICTYPE - Traffic source by which the visitor has arrived at the Web site (e.g., banner, SMS, direct)
- VISITORTYPE - Visitor type as “New Visitor,” “Returning Visitor,” and “Other”
- WEEKEND - Boolean value indicating whether the date of the visit is weekend
- MONTH - Month value of the visit date
- REVENUE - Class label indicating whether the visit has been finalized with a transaction


Notes on Selected Features

(ADMINISTRATIVE, ADMINISTRATIVE_DURATION, INFORMATIONAL, INFORMATIONAL_DURATION, PRODUCT_RELATED, PRODUCT_RELATED_DURATION)
- These features represent the number of different types of pages visited by the visitor in that session and the total time spent in each of these page categories. The values of these features are derived from the URL information of the pages visited by the user and updated in real time when a user takes an action, e.g. moving from one page to another

(BOUNCE_RATE, EXIT_RATE, PAGE_VALUE)
- These features represent the metrics measured by "Google Analytics" for each page in the e- commerce site. The value of "Bounce Rate" feature for a web page refers to the percentage of visitors who enter the site from that page and then leave ("bounce") without triggering any other requests to the analytics server during that session. The value of "Exit Rate" feature for a specific web page is calculated as for all pageviews to the page, the percentage that were the last in the session. The "Page Value" feature represents the average value for a web page that a user visited before completing an e-commerce transaction.

(SPECIAL_DAY)
- This feature indicates the closeness of the site visiting time to a specific special day (e.g. Mother’s Day, Valentine's Day) in which the sessions are more likely to be finalized with transaction. The value of this attribute is determined by considering the dynamics of e- commerce such as the duration between the order date and delivery date. For example, for Valentine’s day, this value takes a nonzero value between February 2 and February 12, zero before and after this date unless it is close to another special day, and its maximum value of 1on February 8.

(OPERATINGSYSTEMS, BROWSER, REGION, TRAFFICTYPE, VISITORTYPE) 
- Attributes of specific user session

Goal is to create a decision tree which can predict class membership of the “Revenue” variable.
