# Part 1- API Automation Instructions

# Tools/Technology Use
- Postman tool
- Framework: Chai BDD

1. Install Postman tool if not already installed
2. Import downloaded json file
3. Click on runner
4. Selection downloaded collection
5. Set delay for 3ms if needed [Not required here]
6. Click on start run

# Command Line run instruction
1. Install node js
2. Install newman
3. npm install newman-reporter-html [for html report generation]

> newman run Part2_CloudCover.postman_collection.json
> newman run Part2_CloudCover.postman_collection.json -r html

# Test Scenarios Covered
1. Status code check
2. Schema check using avj
3. Data Type check 
4. empty response check
5. Invalid badge Id
6. Number of items returned in response
7. Reposne size
8. Response time required
9. Header Check 

[Parametrize Collection ]

I have also creted parametrize colelction where I have parametrize below parameters at collection level
- url
- bid: This the the badge id which will be set from __Get_Badges__ request at collection level, which further will be used under __Get_Badge_ID and __Get_Badge_ID_Recipient__ requests

[Steps to run]
1. Import downloaded json file
2. Create below variable at collection level 
- url: https://api.stackexchange.com
- bid: 5966 [This will be set from __Get_Badges__ request]
3. Click on runner
4. Selection downloaded collection
5. Click on start run
