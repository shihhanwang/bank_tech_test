# Bank tech test
![jasmine_and_console_3](https://user-images.githubusercontent.com/36331920/40427963-144d427c-5e97-11e8-8b44-15f9a5fa957c.png)


## Specification

### Requirements
- You should be able to interact with your code via a REPL like IRB or the JavaScript console. (You don't need to implement a command line interface that takes input from STDIN.)
- Deposits, withdrawal.
- Account statement (date, amount, balance) printing.
- Data can be kept in memory (it doesn't need to be stored to a database or anything).

### Acceptance criteria

- Given a client makes a deposit of 1000 on 10-01-2012
- And a deposit of 2000 on 13-01-2012
- And a withdrawal of 500 on 14-01-2012
- When she prints her bank statement
- Then she would see
```
date || credit || debit || balance
14/01/2012 || || 500.00 || 2500.00
13/01/2012 || 2000.00 || || 3000.00
10/01/2012 || 1000.00 || || 1000.00
```

## My Approach

**Language:** JavaScript

**Testing framework:** Jasmine

First day:
- Write the test ➞ Account balance function
- Write Account balance function ➞ pass the test
- Write the test ➞ Account deposit & history function
- Write Account deposit & history function ➞ pass the test
- Write the test ➞ Account withdraw function
- Write Account withdraw function ➞ pass the test
- Refresher ➞ Account historyUpdate function
- Write the test ➞ Statement print function
- Write Statement print function ➞ pass the test
- Write the test ➞ Account print statement function
- Write Account print statement function ➞ pass the test

Second day(another aproach):
- Write the test ➞ Transaction stores the action & amount & balance & date
- Write Transaction stores the objects ➞ pass the test
- Write the test ➞ transaction History add(transaction) function
- Write  History add function ➞ pass the test
- Write the test ➞ Statement print & add transaction functions
- Write Statement print & add transaction functions ➞ pass the test
- Write the test ➞ Account deposit & withdraw & print statement
- Write Account deposit & withdraw & print statement ➞ pass the test
## Setup

- Clone this repo, run:
`git clone https://github.com/shihhanwang/bank_tech_test.git`

## Usage

- Interact code via JavaScript console, ex:
```javascript
var account = new Account();
account.deposit(5000);
account.withdraw(600);
account.printStatement();
```

## Test

- Open `SpecRunner.html` in browser
