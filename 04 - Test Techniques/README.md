# Test Technique Categories
## Black-Box Testing
- Test basis may include user stories, use cases, and other requirements documentation
- Test cases help detect deviations between the requirements and the implementation
- Coverage is based on the items tested in the test basis but also dependso n the black-box test technique applied
- It cannot be performed at the component level+

## White-Box Testing
- The test basis may include any source of information regarding the structure of the software
- It cannot be performed without relevant programming knowledg
- Coverage is based on the no. items tested within a selected structure
- It can be performed at all test levels

## Experience-Based Testing
- The test bais may include the knowledge and experience of the tester as well as other stakeholders
- Knowledge and experience includes the expected use of the software as well as likely defects
- Commonly combined with white-box and black-box test techniques

## Test Technique Selection
- The purpose of a test technique is to help identify appropriate test conditions, test cases and test data
- Factors
  - Time & Budget
  - Regulatory Standards & Contract Requirements
  - Available Documentation
  - Tester Knowledge & Skill
  - SDLC Model
  - System Complexity
- Formality refers to the level of documentation

# Applying Black-Box Test Techniques

## Equivalence Partitioning
- Values should only belong to one equivalence partition

- Valid partition is the accepted results, invalid for values we want to reject
- Massively reduces test cases
- Can be applied by all test levels
-  Coverage is the no. equivalence partitions tested by at least one value, divided by the total no. identified partitions
- Partitions can be identified for any data element related to the test object
- Invalid partitions should not be tested simultaneously

## Boundary Value Analysis
- Behaviour at the boundaries of equivalence partitions is more likely to be incorrect than the behaviour within the partitions
- Defects more likely to occur near equivalence partition boundaries
- 2 versions (2-point, 3-point)
- Boundary coverage for a partition is measured as the no. boundary values tested divided by the no. identified boundary test values, normally as a %
- Can be applied at all test levels
- Cannot be used if a partition is not ordered

## Decision Table Testing
- A decision table displays business logic in a concise and readable way
- Actions are observable results that are used to verify the expected behaviour
- Decision tables are an effective way of displaying complex logic
- Help prevent important combinations of conditions being missed
- A full decision table has enough tests cases to cover every combination of conditions
- Coverage is measured as the no. decision rules (aka particular combo of conditions) tested by at least one test case divided by the total no. decision rules
- Can be used at all test levels

## State Transition Testing
- State Transition Model Components
  - States
  - Transitions (changes states, triggered by events)
  - Events (inputs)
  - Actions (outputs)
- Often used for menu-based applications and screen navigation testing
- Not suitable for larger systems or systems with non-sequential inputs
- Coverage is measured as the no. identified states or transitions tested divided by the total no. of identified states or transitions

## Use Case Testing
- Post-conditions: conditions that should be met after a use case is completed
- actors - entity that interacts with subject
  - users
  - external hardware
  - other systems (api)
- subject- component/system that a use case is applied
- Use cases describe the interactions of an actor with a subject
- Use cases include exceptional behaviour
- Coverage can be measured by dividing the no. case behaviours by the total. no of use case behaviours

# Understanding White-box Test Techniques

# Statement Testing
- Exercises executable statements in the code
- Coverage is measured as the no. statements executed by the tests divided by the total no. executable statements
- Use flow charts to visualise the control flows of the code

# Decision Testing
- Exercises the decisions in the code
- Coverage is measured as the no. decision outcomes tested divided by total
- 100% decision coverage guarantees 100% statement coverage (this is not vice-versa)

# Utilising Experience-based Test Techniques
- Whose Experience?
  - Testers
  - Developers
  - Users
  - Stakeholders

## Error Guessing
- Attempts to predict the occurrence of defects, errors and failures
- Primarily based on the tester's past experience
- Can be used more methodically using lists

## Checklist-based Testing
- Checklists can result in higher test coverage but lower repeatability compared to formal test cases
- Checklists define test conditions
- Checklists may be based on information from a variety of sources
- Checklists may be re-used
- Can be used for various test types
- Likely to increase test coverage but lower repeatability

## Exploratory Testing
- Testing is carried out within a defined timebox
- Testing is guided by a test charter
- Activities may be documented using session sheets
- When to use
  - Limited documentation
  - Time and budget constraints
  - Combined with other techniques
- Tests are not-defined
- Commonly used within reactive test strategies
- Makes use of time-boxed sessions
- Ideal for when there is only limited documentation available or there are time constraints
