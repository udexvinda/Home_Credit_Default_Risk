# Home_Credit_Default_Risk

<b>Can you predict how capable each applicant is of repaying a loan</b><br/>
<b>Data Source:</b> Home Credit Group<br/>

Data Description

•	application_{train|test}.csv<br/>
o	This is the main table, broken into two files for Train (with TARGET) and Test (without TARGET).<br/>
o	Static data for all applications. One row represents one loan in our data sample.

•	bureau.csv<br/>
o	All client's previous credits provided by other financial institutions that were reported to Credit Bureau (for clients who have a loan in our sample).<br/>
o	For every loan in our sample, there are as many rows as number of credits the client had in Credit Bureau before the application date.

•	bureau_balance.csv<br/>
o	Monthly balances of previous credits in Credit Bureau.<br/>
o	This table has one row for each month of history of every previous credit reported to Credit Bureau – i.e the table has<br/>
(#loans in sample * # of relative previous credits * # of months where we have some history observable for the previous credits) rows.

•	POS_CASH_balance.csv<br/>
o	Monthly balance snapshots of previous POS (point of sales) and cash loans that the applicant had with Home Credit.<br/>
o	This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credits * # of months in which we have some history observable for the previous credits) rows.

•	credit_card_balance.csv<br/>
o	Monthly balance snapshots of previous credit cards that the applicant has with Home Credit.<br/>
o	This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credit cards * # of months where we have some history observable for the previous credit card) rows.

•	previous_application.csv<br/>
o	All previous applications for Home Credit loans of clients who have loans in our sample.<br/>
o	There is one row for each previous application related to loans in our data sample.

•	installments_payments.csv<br/>
o	Repayment history for the previously disbursed credits in Home Credit related to the loans in our sample.<br/>
o	There is a) one row for every payment that was made plus b) one row each for missed payment.<br/>
o	One row is equivalent to one payment of one installment OR one installment corresponding to one payment of one previous Home Credit credit related to loans in our sample.

•	HomeCredit_columns_description.csv<br/>
o	This file contains descriptions for the columns in the various data files.
