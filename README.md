# NIM-App-NIM-OverrideFlags
NIM App - Override Flag Management

# Description
This is an NIM App that provides the ability to manage flags for overriding processing of users. (e.g Skip flags)

# Requirements
- Configure Lookup table
    - Create "OverrideFlags" using provided ["LookupTable_OverrideFlags.csv"](LookupTable_OverrideFlags.csv)
        - Change the Type from "string" to "boolean" for all flags	
	- Add Table to Internal System
	- Set Table Key to "Key"
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
- Key (auto-guid)
- ID
- Type
- Global
- Update
- Disable
- Delete 
- Enable
- NameChange


# Screenshots
![image](https://github.com/user-attachments/assets/1392f98a-83be-457f-a77e-d22dc99fd7da)




# NIM Documentation
The official NIM documentation can be found at: https://docs.nimsuite.com
