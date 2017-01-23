# ACME Bank API - Design exercise

This is a description of ACME Bank's internal APIs.

**Exercise 1: API basics**  
Your task is to design an API based on a set of functional requirements, recorded as user stories.
Start whiteboarding the basics of the API. Focus only on identifying resources (collections and members) and operations.  
_Remember: Resources = nouns, methods = HTTP verbs._  
Remain at this high­ level.

**API Design Requirements**  
"As a bank employee I want to..."
```
[FR-001] Update bank account information
[FR-002] Replace a customer's information
[FR-003] Retrieve details on a particular incoming transfer
[FR-004] Retrieve a list of all transfers, both incoming and outgoing.
[FR-005] Retrieve a full list of customers
[FR-006] Add an account to a customer
[FR-007] Remove an account from a customer
[FR-008] Retrieve a list of a customer’s outgoing transfers
[FR-009] Create an outgoing transfer from a customer’s account to another account
[FR-010] Add a new customer
[FR-011] Retrieve a detailed account report
[FR-012] Get a list of accounts belonging to a particular customer
[FR-013] Retrieve a list of incoming transfers for a particular bank account
[FR-014] Retrieve details on a particular outgoing transfer
```

**Exercise 2: API definition**  
Based on the identified resources and operations, start working on a more elaborate API design.
You may start using a formal API modeling language such as [RAML](http://raml.org).
Create an actual API definition in the [Anypoint API Designer](https://www.mulesoft.com/platform/api/anypoint-designer), [API Workbench](http://apiworkbench.com/)  or any other text editor of choice.
Use the identified resources and operations as a starting point and add the following elements:
* Documentation/API descriptions
* Mediatypes
* HTTP response types
* Sample responses

**Exercise 3: API refinement**  
The last part of this exercise consists of refactoring the API design you created in the previous steps into a full­fledged [RAML](http://raml.org) API:
* Identify possible [traits](http://raml.org/developers/raml-200-tutorial#traits) (reusable behavioural elements). Think of applying paging to large sets of data or searching options. Try to refactor code duplicates into reusable elements.
* Identify data types and data models. Assume all data will be in JSON format. Provide examples in JSON and define [resourcetypes](http://raml.org/developers/raml-200-tutorial#resource-types).
* Review the structure and hierarchy of your API. Apply design recommendations and best practices.

**Exercise 4: API refactoring**
After completing exercise 3, which focused on extracting code duplicates to traits and external examples and schemas, make another pass of your API.
Without the "clutter" of examples etc, see if you can refactor the new API by finding repetitions. Create Resource Types of further of any code duplicates/reperitions.
