# Override Flags

## Description
**Processing Override Management** provides administrators with a centralized interface for managing user processing overrides within NIM. The application allows authorized users to view, create, modify, and remove override flags that influence how automated provisioning and lifecycle processes are executed.

Common use cases include applying skip flags to temporarily exclude users from specific automation workflows, preventing updates during investigations, exceptions, migrations, or other business-driven scenarios. By centralizing override management, the application improves visibility, enhances operational control, and ensures processing exceptions are managed consistently and efficiently across the NIM platform.

# Prerequisites
- [Standard Item Library](https://github.com/Tools4ever-NIM/NIM-Framework-ItemLibrary)

# Installation
- Download app.json source file
- Within NIM
    - Go to Apps
    - Click Import
    - Select app.json
    - Create each missing audit query
    - Complete Import
    - Under Apps, Uncheck "Exportable" if checked
    - Configure Lookup table
    - Create "OverrideFlags" using provided "OverrideFlags.csv"
    	- Key (auto-guid)
		- ID
		- Type
		- Global
		- Update
		- Disable
		- Delete 
		- Enable
		- NameChange
      	- Groups 
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


# Screenshots
<img width="2009" height="1102" alt="image" src="https://github.com/user-attachments/assets/4903591e-1e61-48ad-93d0-5f843174c8ae" />
<img width="2009" height="1102" alt="image" src="https://github.com/user-attachments/assets/439f8115-d524-4326-9a6f-2bc388f09915" />
<img width="2009" height="1102" alt="image" src="https://github.com/user-attachments/assets/1a23c7da-36b8-4a08-80b9-35e806f33556" />
<img width="2009" height="1102" alt="image" src="https://github.com/user-attachments/assets/7480e1c4-3f78-4445-bc19-d1d1cd9f4c54" />






