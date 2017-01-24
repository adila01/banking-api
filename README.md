# ACME Bank - API design exercise

These exercises are part of the [Anypoint Platform Development API Design](https://training.mulesoft.com/instructor-led-training/apdev-api-design) and [Anypoint Platform Architecture Solution Design](https://training.mulesoft.com/instructor-led-training/aparch-solution-design) training courses.

The goal is to design an API based on a set of requirements. Your task is to translate the requirements into an API design and document the design using the [RAML](http://raml.org) language.

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
[FR-015] Retrieve details on a particular customer
```

**Exercise 1: API basics**  
Start white-boarding the basics of the API. 
* Focus only on identifying resources (both collections and members) and methods.  
* Remember: Resources = nouns, methods = HTTP verbs.
* Remain at this high­ level.

**Exercise 2: API definition with RAML**  
Based on the identified resources and operations, start working on a [RAML](http://raml.org) based API definition.  
* Create an actual API definition in the [Anypoint API Designer](https://www.mulesoft.com/platform/api/anypoint-designer), [API Workbench](http://apiworkbench.com/), or any other text editor of choice.
* For now, only add resources and methods.

**Exercise 3: API refinement**  
Use the identified resources and operations as a starting point and add the following elements:
* Documentation/API descriptions
* Media types
* HTTP response types
* Sample [responses](http://raml.org/developers/raml-100-tutorial#enter-responses). Assume all data will be in JSON format.

**Exercise 4: further API refinement**  
This exercise consists of refactoring the API design you created in the previous steps into a full ­fledged [RAML](http://raml.org) API:
* Identify possible [traits](http://raml.org/developers/raml-200-tutorial#traits) (reusable behavioral elements). Think of applying paging to large sets of data or searching options.
* Provide [schemas](http://raml.org/developers/raml-200-tutorial#extract-schemas) for data elements, such as API responses and request bodies. Hint: schemas can be [generated](http://jsonschema.net/#/) from your sample data.
* Review the structure and hierarchy of your API. Apply design recommendations and best practices.
* Extract all defined traits, samples and schemas into external files, which can be referenced using the [include](http://raml.org/developers/raml-200-tutorial#includes) keyword.

**Exercise 5: API refactoring**  
After completing exercise 4, which focused on extracting code duplicates to traits and external examples and schemas, make another pass of your API. Without the "clutter" of examples etc, see if you can refactor the new API by finding repetitions.
* Try to refactor code duplicates/repetitions into reusable elements, such as [resource types](http://raml.org/developers/raml-200-tutorial#resource-types).
* Try to minimize the amount of code in the main RAML file. How much can be extracted into separate resource types, preferably stored in external files?
