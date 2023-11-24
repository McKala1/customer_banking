## customer_banking


## Overview

*  First, I downloaded all of the starter files to my computer so I could open, and work with them in Visual Studio Code. Of course I also made a repository on my GitHub called "customer_banking" to push my assignment to. 

* Second, I opened the "savings_account.py file and imported the "Account" class from the "Accounts.py" file. Then I defined a dunction for the Savings Account that looks like the following "def create_savings_account(balance, interest_rate, months):
    """Creates a savings account, calculates interest earned, and updates the account balance.

    Args:
        balance (float): The initial savings account balance.
        interest_rate (float): The APR interest rate for the savings account.
        months (int): The length of months to determine the amount of interest.

    Returns:
        float: The updated savings account balance after adding the interest earned.
        And returns the interest earned.
    """
* Third, I created an instance for the 'Account' class and passed in the balance and interest parameters. It looks as the following "savings_account = Account(balance, 0)". Then, I calculated the interest earned and subbed in "interest_rate" for the word "apr". It looks as the following "interest_earned = balance * (interest_rate/100 * months/12)". Next, I updated the savings account balance by adding the interest earned, it looks as following "interest_variable = (balance + interest_earned)". Then, I passed the "updated_balance" to the set balance method using the instance of the SavingsAccount class, and used "intered_variable" because it is the updated balance. This looks as the following "savings_account.set_balance(interest_variable)". Lastly, I passed the "interest_earned" to the set interest method using the instance of the SavingsAccount class, it looks as the following "savings_account.set_interest(interest_earned)". To wrap everything up I returned the updated balance and interest earned. It looks as the following "return interest_variable, interest_earned". 
* Fourth, I opened up the "cd_account.y" file and did everything exactly the same as in the steps above. The only thing I did different was set the "def" to be "creat_cd_account" instead of having it as "create_savings_account", and updated the "Returns" float to be the updated CD account balance. It looks as the following "def create_cd_account(balance, interest_rate, months):
    """Creates a CD account, calculates interest earned, and updates the account balance.

    Args:
        balance (float): The initial CD account balance.
        interest_rate (float): The APR interest rate for the CD account.
        months (int): The length of months for the CD.

    Returns:
        float: The updated CD account balance after adding the interest earned.
        And returns the interest earned.
    """

* Lastly, I opened up the "customer_banking.py" and imported the two functions I have been working on. It looks as the following "from cd_account import create_cd_account ; from savings_account import create_savings_account". Then I defined the main function, that looks like this "def main():
    """This function prompts the user to enter the savings and cd account balance, interest rate,
    and the length of months to determine the interest gained.
    It displays the interest earned on the savings and CD accounts and updates the balances.
    """
* From there, I used a float and prompted the user to set the savings balance, interest rate, and months for the savings account. This looks as the following "savings_balance = float(input("Enter the initial savings balance: $ "))
    savings_interest = float(input("Enter the annual interest rate (as a decimal): "))
    savings_maturity = float(input("Enter the number of months for the savings account: "))". Then, I called the create_savings_account function and pass the variables from the user. With this I created a new function that looks as the following "updated_savings_balance, interest_earned = create_savings_account(savings_balance, savings_interest, savings_maturity)". Then with a bunch of print statments and "f" strings I printed out the interest earned and updated savings account balance with interest earned for the given months. This looks as the following "print("\nSavings Account Information:")
    print(f"Interest Earned: ${interest_earned}")
    print(f"Updated Savings Balance: ${updated_savings_balance}")
    print(f"Number of Months: {savings_maturity}")". I then had to set the balance, interest rate, and maturity for the CD account. I used some floats and this looks as the following "cd_balance = float(input("Enter the initial CD balance: $ "))
    cd_interest = float(input("Enter the annual interest rate (as a decimal): "))
    cd_maturity = int(input("Enter the number of months for the CD account: "))". I used the input statment so it would show up for the user to tell them what to do. Next, I had to make a new call for the updated "cd account" and this looks as the following "updated_cd_balance, interest_earned = create_cd_account(cd_balance, cd_interest, cd_maturity)". 

* Lastly, I made some print statments with "f" strings to let the user know what their "cd account" information is and it looks as the following "print("\nCD Account Information:")
    print(f"Interest Earned: ${interest_earned}")
    print(f"Updated Savings Balance: ${updated_cd_balance}")
    print(f"Number of Months: {cd_maturity}")". Then I typed "if __name__ == "__main__":" and called the main funtion "main()". That finished up the purpose of the code. 














