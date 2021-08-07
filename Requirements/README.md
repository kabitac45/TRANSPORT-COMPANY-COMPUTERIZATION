A transport company wishes to computerize various book keeping activities associated with its operations. A transport company owns a number of trucks. The transport company has its head office located at the capital and has branch offices at several other cities. The transport company receives consignments of various sizes at (measured in cubic meters) its different offices to be forwarded to different branch offices across the country.

Once the consignment arrives at the office of the transport company, the details of the volume, destination address, sender address, etc. are entered into the computer. The computer would compute the transport charge depending upon the volume of the consignment and its destination and would issue a bill for the consignment. Once the volume of any particular destination becomes 500 cubic meters, the computerization system should automatically allot the next available truck. A truck stays with the branch office until the branch office has enough cargo to load the truck fully.

The manager should be able to view the status of different trucks at any time. The manager should be able to view truck usage over a given period of time. When a truck is available and the required consignment is available for dispatch, the computer system should print the details of the consignment number, volume, sender's name and address, and the receiver's name and address to be forwarded along with the truck. The manager of the transport company can query the status of any particular consignment and the details of volume of consignments handled to any particular destination and the corresponding revenue generated.

The manager should also be able to view the average waiting period for different consignments. This statistics is important for him since he normally orders new trucks when the average waiting period for consignments becomes high due to non-availability of trucks. Also, the manager would like to see the average idle time of the truck in the branch for a given period for future planning.

Major Entities: trucks management, offices, consignments etc.

Major functionalities: consignment details, status of the consignments, truck details etc.

# Requirements- 

Process: printing the consignment details queried with the consignment id by manager.
Output: status of any particular consignment and the details of volume of consignments handled to any particular destination and the corresponding revenue generated.

R1: updating consignment details.
Input: consignment id and volume (measured in cubic meter), senders address, destination address
Process: updating consignment details in database.
Output: None.

R2: Billing.
Input: volume, destination address, sender address.
Process: computing the transport charge depending upon the volume of the consignment and the distribution 
Output: bill for the consignment.

R3: Allocating truck.
Input: volume of consignments.
Process: system automatically allocate the truck until total volume of truck reaches 500 cbm, then new allocation.
Output: None.

R4: Checking status of trucks at a given time and over a period of time.
Input: current location, starting point, time interval. 
Process: updating database regarding truck’s status.
Output: status of truck.

R5: Print details of consignment and truck on availability before dispatch. 
Input: consignment id, volume, senders address and name, receivers address and name, truck id
Process: print details.
Output: the details of the consignment number, volume, sender's name and address, and the receiver's name and address to be forwarded along with the truck.

R6: Facility for the manager to check Consignment details.
Input: consignment id.

R7: Manager can check the average waiting time of consignment.
Input: consignment id. Dispatch time, issued time
Process: Calculate the average waiting time
Output: Average waiting time for different consignment.

R8: Order new Truck
Input: average waiting time
Process: Order a new truck if average wait time is greater than threshold, if yes then order new truck
Output: print new truck id

R8: Average idle time for truck at a branch.
Input: Truck id, branch id, truck issue time, truck time dispatch time
Process: Calculate the average idle time for a truck
Output: Print Average idle time.






