# Home_Credit_Default_Risk\
# Can you predict how capable each applicant is of repaying a loan?\
# Data Source: Home Credit Group\

Data Description

•	application_{train|test}.csv

o	This is the main table, broken into two files for Train (with TARGET) and Test (without TARGET).
o	Static data for all applications. One row represents one loan in our data sample.

•	bureau.csv
o	All client's previous credits provided by other financial institutions that were reported to Credit Bureau (for clients who have a loan in our sample).
o	For every loan in our sample, there are as many rows as number of credits the client had in Credit Bureau before the application date.

•	bureau_balance.csv
o	Monthly balances of previous credits in Credit Bureau.
o	This table has one row for each month of history of every previous credit reported to Credit Bureau – i.e the table has (#loans in sample * # of relative previous credits * # of months where we have some history observable for the previous credits) rows.

•	POS_CASH_balance.csv
o	Monthly balance snapshots of previous POS (point of sales) and cash loans that the applicant had with Home Credit.
o	This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credits * # of months in which we have some history observable for the previous credits) rows.

•	credit_card_balance.csv
o	Monthly balance snapshots of previous credit cards that the applicant has with Home Credit.
o	This table has one row for each month of history of every previous credit in Home Credit (consumer credit and cash loans) related to loans in our sample – i.e. the table has (#loans in sample * # of relative previous credit cards * # of months where we have some history observable for the previous credit card) rows.

•	previous_application.csv
o	All previous applications for Home Credit loans of clients who have loans in our sample.
o	There is one row for each previous application related to loans in our data sample.

•	installments_payments.csv
o	Repayment history for the previously disbursed credits in Home Credit related to the loans in our sample.
o	There is a) one row for every payment that was made plus b) one row each for missed payment.
o	One row is equivalent to one payment of one installment OR one installment corresponding to one payment of one previous Home Credit credit related to loans in our sample.

•	HomeCredit_columns_description.csv
o	This file contains descriptions for the columns in the various data files.
