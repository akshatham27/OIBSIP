# Simple Banking Application in Java


Overview
This project is a simple banking application written in Java. It simulates basic operations for a savings account, including account creation, deposit, withdrawal, and viewing transaction history. The application handles multiple accounts and ensures valid transactions through custom exception handling.

Project Structure
The project is structured into several classes, each with specific responsibilities:

1. op Class
Description:
Acts as the main class that manages the banking system.
Contains a static variable to track the total number of accounts created.
Includes inner classes (acc, SavingsAccount) and a custom exception class (InvalidTransactionException).
2. acc Class (Account)
Description:

Represents a generic bank account with attributes such as name, accno (account number), balance, history (transaction history), and acctype (account type).
Provides methods to perform account operations like deposit, withdrawal, and viewing transaction history.
Key Methods:
deposit(double amount): Deposits a specified amount into the account.
withdraw(double amount): Withdraws a specified amount from the account.
printHistory(): Prints the transaction history of the account.

3. SavingsAccount Class
Description:
A subclass of acc that represents a savings account.
Inherits all features from acc and is specifically tailored for savings accounts.
Note: This class currently doesn’t include interest application, focusing on basic deposit and withdrawal functionality.

5. InvalidTransactionException Class
Description:
A custom exception class to handle invalid transactions.
Throws exceptions for actions like attempting to deposit a non-positive amount or withdrawing more than the available balance.



How It Works
1. Account Creation
Users are prompted to input their name, account number, and initial deposit.
A new SavingsAccount object is created with the provided details.
The account information and initial balance are displayed.
2. Transactions
Users can:
Deposit: Add funds to their account. The balance is updated, and the transaction is recorded.
Withdraw: Remove funds from their account. The balance is checked to ensure sufficient funds before processing the transaction.
The updated balance is displayed after each transaction.
3. Transaction History
Users can view the transaction history for their account, showing all deposits and withdrawals.
4. Summary
The application displays the total number of accounts created during the session.
Exception Handling
The program includes robust exception handling:

InvalidTransactionException: Ensures that only valid transactions are processed, with appropriate error messages displayed for invalid actions.
How to Run the ApplicatioN

Input your details to create an account.
Perform transactions such as deposit and withdrawal.
View your transaction history.
Future Enhancements
Interest Calculation: Implement interest calculation for savings accounts.
Multiple Account Types: Support additional account types (e.g., checking, fixed deposits).
Graphical User Interface (GUI): Develop a GUI for better user interaction.
Data Persistence: Implement database or file storage to retain account data across sessions.


Contributions are welcome! Please fork this repository and submit a pull request with your changes. Ensure that your code follows the project’s style and passes all tests before submitting.
