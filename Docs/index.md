# Tutorial: FireCode

FireCode is a platform for honing your coding skills. You can **create an account** to track your progress and *login* to access features. Explore a variety of **coding problems**, each with a description and related information. Write and **submit your code** solutions, and the platform will *automatically test* them against predefined cases, giving you *feedback* like "Accepted" or "Wrong Answer". All your *account details, problem status, and submission history* are persistently stored for you.


**Source Repository:** [https://github.com/coderhuBypassion/FireCode](https://github.com/coderhuBypassion/FireCode)

```mermaid
flowchart TD
    A0["User Authentication and Accounts"]
    A1["Problem Management"]
    A2["Code Execution and Submission"]
    A3["API Routing]
    A4["Frontend Pages and Navigation"]
    A5["Data Persistence (MongoDB/Mongoose)"]
    A6["Middleware"]
    A7["UI Components"]
    A8["Utility Functions"]
    A4 -- "Talks to API" --> A3
    A3 -- "Routes to Auth Logic" --> A0
    A3 -- "Routes to Problem Logic" --> A1
    A3 -- "Applies Middleware" --> A6
    A3 -- "Connects to DB" --> A5
    A0 -- "Manages User Data" --> A5
    A1 -- "Manages Problem Data" --> A5
    A0 -- "Requires Auth" --> A6
    A1 -- "Triggers Execution For" --> A2
    A2 -- "Uses Execution Utils" --> A8
    A4 -- "Composed of Components" --> A7
    A7 -- "Uses Rendering Utils" --> A8
    A0 -- "Uses Auth Utils" --> A8
    A1 -- "Uses Problem Utils" --> A8
    A5 -- "Uses Type Definitions From" --> A8
```

## Chapters

1. [Frontend Pages and Navigation](01_frontend_pages_and_navigation_.md)
2. [UI Components](02_ui_components_.md)
3. [User Authentication and Accounts](03_user_authentication_and_accounts_.md)
4. [Code Execution and Submission](04_code_execution_and_submission_.md)
5. [Problem Management](05_problem_management_.md)
6. [Data Persistence (MongoDB/Mongoose)](06_data_persistence__mongodb_mongoose__.md)
7. [Middleware](07_middleware_.md)
8. [API Routing](08_api_routing_.md)
9. [Utility Functions](09_utility_functions_.md)
