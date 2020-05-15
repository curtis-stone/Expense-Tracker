# Expense-Tracker
Make it simple to keep track of your bank account by using these JavaScript methods

//primary account object
let myAccount = {
    name:'CJ',
    expenses: 0,
    income: 0,
};

// add income amount to account's income property
function addIncome(account, income) {
    account.income = account.income + income;
};

// add expense amount to account's expense property
function addExpense(account, expenses) {
    account.expenses = account.expenses + expenses
};

// resets account data to 0
function resetAccount(account) {
    account.income = 0;
    account.expenses = 0;
}

function getBalance(account) {
    balance = account.income - account.expenses;
    return balance;
};

// summarizes account information such balance, income, and expenses
function getAccountSummary(account) {
    let balance = (account.income) - (account.expenses);
    return `The Account for ${account.name} has a balance of $${balance}, 
    $${account.income} in income, and $${account.expenses} in expenses.`;
};

 addIncome(myAccount, 2000) // adds income to account
 getBalance(myAccount) // returns the balance of the account (income-expenses)
 console.log(getBalance(myAccount)) // prints balance to console
 addExpense(myAccount, 2.50) // adds to expenses proprty in myAccount object
 addExpense(myAccount, 160)
 getAccountSummary(myAccount) // returns a detailed summary of each property of myAccount
 console.log(getAccountSummary(myAccount)) // prints summary to console
 resetAccount(myAccount) // resets all values in myAccount to 0
 console.log(getAccountSummary(myAccount)) // prints the new values, after the reset, in the console
