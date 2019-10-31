# R-Programming-Code
Dplyr and other code
# INRODUCTION TO R-PROGRAMMING ASSIGNMENT
Customer_Churn <- read.csv("Customer_Churn.csv", TRUE, ",")

# a.	Add 5 to the fifth record of 'MonthlyCharges' column

Customer_Churn$MonthlyCharges[5]  #show current value
Customer_Churn$MonthlyCharges[5] <- Customer_Churn$MonthlyCharges[5]+5  #addition
Customer_Churn$MonthlyCharges[5]    #added value

#b.	Subtract 9.65 from the sixth record of 'MonthlyCharges' column
Customer_Churn$MonthlyCharges[6]  #show current value
Customer_Churn$MonthlyCharges[6] <- Customer_Churn$MonthlyCharges[6] - 9.65
Customer_Churn$MonthlyCharges[6]  #show subtracted value

#c.	Multiply the 1st record of 'MonthlyCharges' column with 3
Customer_Churn$MonthlyCharges[1]
Customer_Churn$MonthlyCharges[1] <- Customer_Churn$MonthlyCharges[1] * 3
Customer_Churn$MonthlyCharges[1]

#d.	Divide the 37th record of 'MonthlyCharges' column with 3
Customer_Churn$MonthlyCharges[37]
Customer_Churn$MonthlyCharges[37] <- Customer_Churn$MonthlyCharges[37]/3

# Working with the relational operators
a.	Checking if the value of 'tenure' in the 1st row is greater than the value of 'tenure' in the 10th row

Customer_Churn$tenure[1] > Customer_Churn$tenure[10]

#Checking if the value of 'tenure' in the 3rd row is equal to the value of 'tenure' in the 5th row

Customer_Churn$tenure[3] == Customer_Churn$tenure[5]


# Working with logical operators:
# a.	Count of customers who have subscribed to both "TechSupport" & "StreamingTV"
count_tech <- Customer_Churn$TechSupport == "Yes" & Customer_Churn$StreamingTV == "Yes"
count_tech

# Extract those customers whose 'InternetService' is either 'DSL' or 'Fiber optic'

count_dslorfiber <- Customer_Churn$InternetService == "DSL" | 
                    Customer_Churn$InternetService == "Fiber optic"
count_dslorfiber



