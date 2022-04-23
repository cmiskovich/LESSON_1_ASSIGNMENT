# LESSON_1_ASSIGNMENT
This repository is created for Lesson 1 due April 24th, 2022 for GW Fintech Boot Camp.  
The purpose of this assignment is to create a loan analyzer in python using  calculations that analyze data from hypothetical set of dictionaries and lists.  Also, in this assignment you create a conditional filter from a set of lists based on if else statements and then capture the condtitional filter in an empty list and save the results to a comma seperated file (csv).

##  Section 1 - *Automate the Calculations*

        The following data is given:
        loan_costs = [500, 600, 200, 1000, 450]

###        1. Using the len function and referencing loan costs I was able to determine that the nubmer of loans are 5 and create a calculation called number_of_loans. My code for this is on line 22.

###        2. Using the sum function and referencing loan costs I was able to determing the total value of the loans are $2750 and create a calculation called total_value.  My code for this is on line 29.

###        3. Using my previous 2 calculations I am able to create a thrid called average_loan_amount.  This is done by dividing The number_of_loans by the total_value.  My code fo this is on line 36.

###        4. I was able to print the three calculations with descriptive messages and the code is on lines 23, 30, and 37.

###            When the program is run the following data appears:
                The number of loans are 5.
                The total value of the loans are 2750.
                The average amount of the loans are 550.00.
    

##  Section 2 - *Analyze Loan Data*

        The following data is given:
                loan = {
                        "loan_price": 500,
                        "remaining_months": 9,
                        "repayment_interval": "bullet",
                        "future_value": 1000,
                        }

###        1. Using the get() I was able to extract the future value and remaining months on the loans dictionary listed above and save them as variables future_value and remaining months.  I am also able to print the values running the program. My code is on lines 75 to 77.  

###            When the program is run the following data appears:
                Future value = 1000 and remaining months = 9

###        2. Using the amounts in the loan dictionary and a return rate of 20% I used the present value formula to create a calculation called fair_value.  I am also able to print the fair_value running the program.  My code is on lines 85 and 86.

###             When the program is run the following data appears:
                The present value of the loan is $ 861.77.

###        3. I prepared and if-else statement with the condition that represents the loans fair value compared to the present value.  If the present value of the loan is greater than or equal to the cost, then print a message that says that the loan is worth at least the cost to buy it. If the present value of the loan is less than the loan cost, then print a message that says that the loan is too expensive and not worth the price. My code is on lines 93 - 96.  I am also able to print the result when the program is run.

###            When the program is run the following data appears:
               The loan is worth at least the cost to buy it.


##  Section 3 - *Perform Financial Calculations*


            The following data is given:

                    new_loan = {
                                "loan_price": 800,
                                "remaining_months": 12,
                                "repayment_interval": "bullet",
                                "future_value": 1000,
                                                        }

###            1. Define a new function to calculate present value and the function should meet the following criteria:
###                a. future_value, remaining_months, and the annual_discount_rate: this is done with my code on line 125 and 126.  (The discount rate was added to the list on line 118.)
###                b. Return the present_value for the loan.  This is done with my code on line 127,

###            2. I used the function to print the present value of the new loan and that code is on lines 132 and 133.

###                When the program is run the following data appears:
                  The present value of the loan is:  820.08.     

##  Section 4 - *Conditionally Filter Lists of Loans*

###            1. I created a new empty list and named it inexpensive_loans on line 175.

###            2. I used a for loop to determine which loans were less than or equal to $500 by loan_price this code is on line 181 and 183.

###            3. I then appended the loan if it met the criteria and added it to the inexpensive loan list this code is on line 185.

###            4. I have a line of code to print the inexpensive_loan list on line 192.

###                When the program is run the following data appears:
                    The list of inexpensive loans [{'loan_price': 500, 'remaining_months': 13, 'repayment_interval': 'bullet', 'future_value': 1000}, {'loan_price': 200, 'remaining_months': 16, 'repayment_interval': 'bullet', 'future_value': 1000}]



##  Section 5 - *Save the Results*     

###            1. I used open to open a new CSV file, then created a csvwriter using the csv library, after that used the new csvwriter to write the header variable as the first row. Then wrote a for loop to iterate through each loan in inexpensive_loans. Finally used the csvwriter to write the loan.values() to a row in the CSV file.  My code for this is in lines 210 - 227.

###                The output of this function is a file called inexpensive_loans.csv and the link is below.

[Inexpensive Loans](inexpensive_loans.csv)



