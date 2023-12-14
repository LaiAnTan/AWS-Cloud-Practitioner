
#concept #module_2 

A **tightly coupled** architecture refers to components that communicate with each other directly in an application.

- If one component fails, others fail as well
- considered a **monolithic application**

A **loosely coupled** architecture refers to components that are standalone and individual.

- If one component fails, others will not fail
- Considered a **microservices approach** ^fb3e59

[[Amazon Simple Notification Service (SNS)]] and [[Amazon Simple Queue Service (SQS)]] are two of the tools that can be used to in an application with a microservices approach to facilitate application integration.

[[Amazon EventBridge]] also can be used to facilitate application integration.