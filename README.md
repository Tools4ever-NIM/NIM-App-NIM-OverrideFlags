# NIM-App-NIM-OverrideFlags
NIM App - Override Flag Management

# Description
This is an NIM App that provides the ability to manage flags for overriding processing of users. (e.g Skip flags)

# Requirements
- Configure Lookup table
    - Create "OverrideFlags" using provided ["LookupTable_OverrideFlags.csv"](LookupTable_OverrideFlags.csv)
	- Add Table to Internal Users
	- Create Inter-System relation
		- System A
			- System: internal
			- Table: OverrideFlags
			- Column: ID
		- System B
			- System: AD
			- Table: Users
			- Column: employeeID

# Configuration
A lookup table is required with the following columns
- ID
- Type
- Global
- Update
- Disable
- Delete 
- Enable
- NameChange


# Screenshots
![image](https://user-images.githubusercontent.com/24281600/233438244-0985545a-484e-4ebc-9aab-02c5778db462.png)


![image](https://user-images.githubusercontent.com/24281600/233438269-b07321bb-8a0f-4dd4-a16d-3e00e0d0223e.png)



# NIM Documentation
The official NIM documentation can be found at: https://docs.nimsuite.com
