Objective
Design an automated system to manage the allocation of time blocks in a calendar based on availability, capacity rules, and client confirmation.

Functional Requirements
Types of Time Blocks:

Type 1: Reserve 1-hour blocks (with specific capacity rules).
Type 2: Reserve 2-hour blocks (the closest available option).
Type 3: Reserve 6-hour blocks (the closest available option).
Operating Hours:

Working days: Monday to Friday.
Available hours:
Morning: 08:00 AM - 02:00 PM.
Afternoon: 04:00 PM - 08:00 PM.
Weekly Capacity (only for Type 1):

The system has 4 available resources (people, machines, or rooms).
The total capacity is 160 hours per week.
Type 1 blocks will be assigned within the current week as long as the total usage does not exceed 80% of the weekly capacity.
If the usage exceeds 80%, the blocks will be assigned to the following week.
Immediate Assignment (Types 2 and 3):

For Type 2 and Type 3 blocks, the closest available option will always be selected, without considering weekly capacity.
Non-Working Days:

Blocks will not be assigned on non-working days (defined in an external holiday calendar).
Prior Confirmation:

Before assigning a block, the system must inform the client of the available options.
A block will only be reserved once the client confirms their choice.
Flow Functionality
Step 1: Identify the Type of Block
The client specifies whether they need a block of 1, 2, or 6 hours.
Step 2: Check Availability
The system analyzes the available time blocks in the calendar, taking into account:
Operating hours.
Non-working days.
Required duration.
For Type 1: Check weekly capacity.
For Types 2 and 3: Find the closest available block.
Step 3: Verify Capacity (only for Type 1)
If the weekly capacity usage is below 80%, options within the current week are assigned.
If the weekly capacity usage is above 80%, options are searched for in the following week.
Step 4: Inform the Client
The client receives a list of available blocks for the required time.
The client is asked to confirm their preferred option.
Step 5: Reserve the Block
Once the client confirms, the system registers the block in the calendar with the corresponding details.
Let me know if you need additional changes or more details!
