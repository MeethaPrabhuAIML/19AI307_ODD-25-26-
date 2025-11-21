# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
A jewelry store tracks gold rates for different types of customers. The base class is Customer with attributes like customerId, name, and purchaseWeight (in grams). There are two types of customers: RegularCustomer and PremiumCustomer. RegularCustomer gets a fixed discount of 2% on the gold rate per gram. PremiumCustomer gets a 5% discount plus a special cashback. The base gold rate per gram is input at runtime. For each customer, calculate the final price they pay:

finalPrice = purchaseWeight * (goldRatePerGram - discount)

## AIM:
To write a program to calculate the final bill amount for Regular and Premium customers based on gold rates and their specific discounts.


## ALGORITHM :
1. Start the program.

2. Import the necessary packages 'java.util' and 'java.text'.

3. The program waits for the user to enter the customer type, ID, name, purchase weight, and gold rate per gram.

4. The program checks the customer type provided.

5. If the type is "Regular", it creates a RegularCustomer object (which applies a 2% discount).

6. If the type is "Premium", it creates a PremiumCustomer object (which applies a 5% discount and calculates cashback).

7. If the type is neither, it creates a standard Customer object (with 0% discount).

8. The program calls the display method to calculate the final price using the formula: weight * (rate - discount).

9. The program prints the customer details, the calculated final price, and the cashback amount (only if the customer is Premium).

10. End the program.


## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:







## OUTPUT:



## RESULT:

