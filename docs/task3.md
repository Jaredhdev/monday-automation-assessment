## Task 3: Identifying Null Priorities

**Objective**: Find items without a priority value assigned using Make.com.

### Step 1: Fetch and Filter Columns
Make.com calls Monday.com's API and retrieves only these columns:
- `Name` (column ID: `name`)
- `Status` (column ID: `status`)
- `Priority` (column ID: `priority`)

![3.1](screenshots/3.1.png)

### Step 2
A filter lets items pass through based on the condition:
- `Priority does not exist`

![3.2](screenshots/3.2.png)

### Step 3
A Set Variable module extracts:
- `Status`: Current item status
- `Priority`: Empty value (shown as `null`)

![3.3](screenshots/3.3.png)