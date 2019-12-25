## 
- 2 accounts, account1, account2
- transfer $1 account1 -> account2, $2 account2 -> account1
- concrrency 2k?
- verify result

## a stream source
- either new records in a table or files dropped in one folder

## 
- transaction history for each account

## the state held within Flink can be accessed via a REST API

## understand how flink works in cluster
- how to know which transaction is executed on which node
- how to devide work to differnt nodes

## 
- account1
- half transaction, either debit from account1 or credit to account1, $1 each time
- concurrency 20k
- verify result

## 
- 10K? accounts
- transfer random amounts between random accounts 
- concurrency
- verify result

## add the stop and retry logic
- stop the transaction if the amount is greater than the debit account balance
- retry the transaction after next credit transaction 

## disaster recovery
- stop the process when it is running

## TODO
- These requirements for timely stream processing can be met by using event-time timestamps that are recorded in the data stream, rather than using the clocks of the machines processing the data.
- 