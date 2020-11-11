Name: Patel Tejas	 	UTA ID: 1001729131
Name: Jariwala Prayag 	UTA ID: 1001719373

Mongodb collection is used in the program as a data structure

In order to to run the program user must download and install mongodb community server edition.

The program uses pymongo librabries, in order to install pymongo user must execute the following commmand on command prompt
>pip install pymongo

The input is given as a textfile. user can give file name on line 9.
The output is generated as a text file. user can specify filename on line 16.

In order to run the program user must execute following command on command prompt.

>python project1.py

Output format:

At every statement in input file new timestamp is generated, so It may be possible that the transaction ID and timestamp are not same but the criteria of having a greater timestamp for the older transactions than the younger transactions is fullfilled.

in the output, two tables are generated

1) Transaction table:

	T_ID : Represent ID of the transaction
	TimeStamp : Represents the timestamp when the transaction is created
	State: Reperesents state of transaction (active, waiting(blocked), aborted, commited)

2) Lock Table:

	DataItem : Represents the item
	Lock_mode : Represents that under which mode the dataitem is locked (read or write).
	T_Id_List : Represents hwo many transaction is holding the dataitem under whuch order.
	BlockedOperation : Represents blocked operation for the dataitem
						(r2 - means read operation is blocked for transaction no 2.)

sample input files and corresponding output files are provided in the folder.

Efforts:

learned mongodb together.
the logic for write and end operations is developed by Patel Tejas
the logic for begin and read operations is developed by Jariwala Prayag
The whole code is developed together.


