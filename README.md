# Map-Reduce-Program-for-finding-Flight-Connections-
You can download the dataset from the following URL: 
https://uofi.box.com/s/ovfo5ps7a9bafu725hffevonn0xpte5e 

We need to write a MapReduce program to find all pairs of distinct  flights with path lengths two, that is all pairs of flights F1 and F2 where F1 flies from A to B and F2 flies from B to C (where C is not equal to A). For example, F1 flies from Chicago to Atlanta and F2 flies from Atlanta to Boston
 F1 and F2 must also satisfy the following additional conditions: 
1. F1 and F2 both have the same unique carrier 
2. F1 and F2 both depart on the same date ( i.e., they have the same year, month, and day of the month)
3. F2’s scheduled departure time is at least 1 hour and at most 8 hours after the F2’s scheduled arrival time ( that is, they must have a layover or at least one and at most eight hours). 
4. None of the flights have  been cancelled ( that is, the cancelled column should not be equal to 1) 
 
Each line of the output of your MapReduce program should have the following format: 
Year/month/day F1’s flight number F2s flight number F1’s origin F1’sdestination     F2’s destination F1’s scheduled arrival time F2’s scheduled departure time 

The zip file has source code which includes Mapper, reducer, and driver classes. Driver class is FlightDriver.java

To run the code copy the full dataset to your Hadoop distributed file system. Then run your program for the entire dataset on yarn cluster.
