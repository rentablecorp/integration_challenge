# Integration Challenge
The goal of this challenge is to create a python script that will retrieve and parse a tenant's ledger from Yardi and return their balance and if they are ready for disbursement.

A tenant can have two types of transactions:
* Charges need to be payed by the tenant. They increase the balance.
* Payments are made by the tenant. They decrease the balance.

There are two requirements for a tenant to be ready for disbursement:
* The tenant must have an IDType of "Past"
* The tenant must have a transaction with a Note that includes the substring ":Prog Gen"

If either of these criteria are not met, the tenant is not ready for disbursement.

The endpoint to get the tenant ledger is "http://integration.tryrentable.com".

Please have your script be runnable from the commandline and print out a tuple with the balance and whether or not the tenant is ready for disbursement.

If you create any examples to test your code, please include them in your final project.
