# Date_Script


## Purpose:
The purpose of this script is to simulate a dating scenario and offers an interactive experience for the user. The script will facilitate the following functionalities:




### User Input:

The user will input the name of the person they are on a date with.
The user will specify their budget for the date.
The user will select food and drink items from a restaurant menu list for both themselves and their date.


### Budget Tracking:

The script will keep track of the user's budget and update it after each food or drink item selection. It will also display the remaining budget to the user after each order.



### Payment Confirmation:

At the end of the date, the user will be asked to confirm if they agree to pay the bill.



### Final Budget Display:

After the user agrees to pay the bill, the script will show the user their final budget.



### Second Date Decision:

The script will analyze all the user's inputs, including the date's choices and the budget, to make a decision about whether the user will get a second date or not.


### Issues & Optimization:
*If someone uses a letter (or any non-integer input) when ordering from the menu, it will result in a ValueError. This is because the script expects the user to input an integer representing the quantity of the item they want to order, and it attempts to convert the user's input to an integer using the int() function.
To handle this issue and make the script more robust, I can add error handling using a try and except block.* 

*Another issue was that the budget would reset to its initial value for each new order, instead of keeping track of the cumulative total order cost for each user and their date. To fix this issue, I made the user's total cost and the date's total cost global variables, allowing the function to update the total order cost for both the user and the date.*

* **Please note that using global variables should be done with caution, as it can make code harder to understand and maintain. In many cases, it's better to pass variables as function parameters and return values to promote cleaner and more modular code. However, in this specific scenario where I want to maintain a running total across multiple function calls, using a global variable can be a reasonable choice.** 



