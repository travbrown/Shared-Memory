# Shared-Memory

## Communication between Parent and Child Process via Shared Memory
The program in bank.c creates two shared variables of type int: BankAccount, and Turn. This program creates two processes, one parent process and one child process, and allows the parent to deposit (i.e. add) money to the BankAccount, and also allows the child process to withdraw (i.e. subtract) money from the BankAccount using Tanenbaum’s strict alternation. Both the Parent and Child loop 25 times and follow the rules each time through the loop.

## Here is an example output
Process has recieved shared memory of 2 integers...
Process has attached the shared memory...
Poor Student needs $18
Poor Student: Not Enough Cash ($0)
Dear old Dad: Deposits $68 / Balance = $68
Poor Student needs $3
Poor Student: Withdraws $3 / Balance = $65
... (this alternation for a total of 50 times)
Poor Student needs $28
Poor Student: Withdraws $28 / Balance = $38
Dear old Dad: Deposits $78 / Balance = $116
Process has detected the completion of its child...
Process has detached its shared memory...
Process has removed its shared memory...
Process exits...
