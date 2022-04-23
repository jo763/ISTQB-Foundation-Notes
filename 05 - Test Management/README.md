# Test Manager

## Test Manager Role
 - Writes the test plan
 - Overall responsibility for the test process
 - Test policy: Why you must test brief, concise, organisational level
  - Outlines test process
  - How testing will be evaluated
  - Quality levels
  - Process improvement
 - Test strategy: what you should test, detailed document, depends on context
  - SPACE: Scope, People, Approach, Criteria, Environment
  - Strategies
    - Analytical
    - Model-based
    - Methodical
    - Process compliant
    - Directed (or consultative)
    - Regression averse
    - Reactive
  - Estimating
    - Preparation, analysis and design, write the tests
    - Implementation, automate tests, run tests
    - Evaluate results, log defects, re-test
    - Repeat for the test levels
    - Determine no. test cycles
    - Schedule all the test activities
    - Co-ordinate with product owners, PMs
    - Write the test plan, keep it updated

## Test Environment
  - Production equivalent test lab
  - Advantages
    - Problems in live can be recreated
    - Performance tests are more realistic
    - Live customer data is available
  - Disadvantages
    - Expensive
    - Virtual user license cost more
    - Data must be sanitised
- Questions
 - Able to afford production equivalent severs?
 - What access devices do testers require?
 - Share office network or build new?
 - From where does one source test data?

## How are tests carried out?
- Manuel or automated
- Acquire resources
- Support tool selection
- Defect management
- Configuration management e.g. server settings, version control
- Introduce metrics to monitor and control progress
- Initiate the testing
- Monitor progress
- Check exit criteria
- Report
- Adapt the plans

# Tester

## Tester Role
- Design Test environment
- Reserve test lab
- Co-ordinate with sys admin
- Identify test conditions
- Design and implement test cases and procedutes
- Build test DB
- Prepare the test data
- Create the schedule
- Execute tests
- Use appropriate tools
- Automate some tests (can be supported by a developer)
- Consider the NFRs
- ISO/IEC Standard 25010 - describes a classification of software product quality characteristics (Good for non-functional characteristics)
- NFRs (Quality attributes)
  - Performance
  - Efficiency
  - Reliability
  - Compatibility
  - Usability
  - Portability
  - Security
  - etc.

## Independent Testing
- Can you find defects in own work?
- Degree of tester independence is useful
- Independence doesn't replace familiarity

- Degrees of independence in testing
  1. None
  2. Some independent testers
  3. Independent test team
  4. Business testers
  5. External, independent testers

- Potential benefits of independent testing
  - Recognise different kinds of failures
  - Verify, challenge or disprove assumptions
- Potential drawbacks of independent testing
  - Isolation from the developers
  - Lose responsibility for quality
  - Testers seen as a bottleneck
  - Testers lack critical information
- ISO/IEC Standard 29119-1: has further info about software testing concepts

- Who can test?
  - Professional testers
  - Specialists in security, performance
  - Almost anyone in your organisation

# Product Risk Analysis

## Product risk (quality risks)
- impacts customers
- Examples
  - Software might not perform to spec
  - Software might ignore customer needs (accessibility)
  - Inadequate system architecture
  - Incorrect computations
  - Loops coded incorrectly
  - Slow response times
  - Poor user experience (UX)

## Project risk
- Impacts schedule
- Examples
  - Delays in delivery
  - Inadequate funding
  - Late changes
  - Organisational issues
    - Project resourcing
    - Personnel issues
    - Conflicting business priorities
  - Political Issues
    - Bad attitude
    - Failure to improve practices
    - Poor communication
  - Technical Issues
    - Requirements not well defined
    - Existing constraints
    - Test environment not ready
    - Data migration may be late
    - Variable quality of work products
    - Technical debt
  - Supplier Issues
    - 3rd party fails to deliver
    - Contractual issues
- Test Manager responsibility to help mitigate risks
  - Hire contractors
  - Work overtime
  - Improve the estimates
  - Manage changes

## Calculate Risk Level
- Risk-based Testing (RBT)
- Impact
  - The harm caused if software fails
  - Measured on a scale of 1 to 5
  - All stakeholders provide input
- Likelihood
  - Chance of software failure
  - Measured on a scale of 1 to 5
  - Technical reasons prevail

- Risk helps testers focus their efforts
- Through testing, adverse events are
  - Less likely to happen, or
  - Their impact is reduced
- Testing is a risk mitigation activity

- RBT is a pro-active strategy
- Product risk analysis
- Guides the test planning
- This enables
  - Choose test techniques
  - Select levels and types of testing
  - Determine the depth of testing
  - Prioritise testing
  - Additional activities - provide testing

- Risk Management
  1. Identify risks
  2. Determine importance
  3. Response plan
  4. Contingency plan
  5. Return to 1.
- Risk Management standard: ISO 31000

# Managing Defects

## How to write a defect report
- Why log defects
  - Finding defects is a test objective
  - Defect reports aid resolution
  - Context determines the process
- Defect logging process
  - Start
  - Analysis
  - Track
  - Finish (all test pass?)
- When are defects reported?
  - During coding
  - Static analysis and reviews
  - Dynamic testing
  - Using the product
- where are defects found?
  - in the code
  - in the working software
  - in documentation
- Objectives of defect report
  - Provide info to resolve
  - Feedback on quality
  - Catalyst for improvement

- What do defect report usually contain?
  - ID number
  - Title
  - Summary
  - Date
  - Organisation
  - Author
  - ID of the test/configuration item
  - Status (new, open, closed, blocked etc.)
  - Lifecycle phase
  - Test environment
  - Detailed description (on how to reproduce problem plus expected and actual results)
  - Changed history references
  - Global issues
  - Conclusions, recommendations, approvals

## Defect Management Process
- Defect workflow
  1. New
  2. open
  3. fixing (may reject and go to 6. as unable to reproduce/duplicate defect)
  4. ready
  5. retest --> 2 (as re-open) or 6
  6. closed (may have resolution code)
- Test planning standard ISO/IEC/IEEE 29119-3

### Configuration management
- Without config management
  - Defects that were fixed, reappear
  - Working software suddenly fails
  - Enhancements are tested, then lost
  - Unable to recreate production failures

- Configuration management procedures and tools are identified and implemented during test planning

# How to Write a Test Plan

## Purpose
- Test Planning Influences
  - Test policy - why we must test?
  - Test strategy - What will be tested? what's in scope?
  - Test plan - How is the testing carried out?
  - Development lifecycles and methods
  - Scope of testing
  - Test objectives
  - Risks
  - Constraints
  - Testability
  - Availability of resources
- Test Plans
- Master Test Plan with separate test plans e.g.
  - Unit Test plan
  - System test plan
  - UAT plan
  - Network performance test plan
  - Usability test plan
- Test Planning Activities
  1. Determine the scope
  2. Choose an approach
  3. Integration and coordination
  4. Make decisions about who run tests, what will be tested, and how it will be carried out
  5. Scheduling
  6. Metrics
  7. Budgeting
  8. Templates
  - Test Planning is Continuous, updated throughout the test
  - Test Planning ISO/IEC/IEEE 29199-3

## Test Strategy and Test Approach
- Test strategy depends on context
- Test strategies
  - Analytical (risk-based testing)
  - Model-based (based on model of the software)
  - Methodical (pre-defined test, checklists)
  - Process compliant (tests based on external and industry spec standards)
  - Directed (by (external) experts)
  - Regression Averse (avoid regression issues)
  - Reactive (testing reacts to component being tested e.g. exploratory testing)

## Entry and exit criteria
- Entry - preconditions before starting testing
  - Availability of requirements, stories, models
  - Availability of test items
  - Test environment setup and ready
  - Test database and test data
  - Test tools installed and available for use
- Exit - conditions when testing is done
  - Planned tests have been run
  - Coverage level achieved
  - Unresolved defects
  - Remaining defects low
  Level of quality characteristics
- Testing may be stopped prematurely
  - Budget limit reached
  - Scheduled time used up
  - Product must go to market
  - Release software if
    - All stakeholders accept the risk

# Applying Estimating Techniques
## Test Execution Schedule
- Must balance efficiency of text execution with the test priority
## Factors affecting the test effort
- Product characteristics
  - Product risks
  - Test basis quality
  - Size and complexity
  - Quality characteristics
  - Test documentation detail
  - Legal and regulatory
- People Characteristics
  - Skills, knowledge and experience
  - Team cohesion and leadership
- Development process
  - Organisational maturity
  - Development model
  - Test approach
  - Tools used
  - Test process
  - Time pressure
- Test results
  - No. and severity of defects found
  - Amount of rework required

## Test Estimation Techniques
- Hofstadter's Law - It always takes longer than you expect, even when you take into account Hofstadter's law
1. Metrics-based estimation e.g.
  - Burndown chart
  - Defect removal model
2. Expert-based estimation e.g.
  - Planning poker
  - Wideband Delphi
- Include ALL test activities
- Test preparation is not just test execution
- Defect logging, triage and reporting
- No. test cycles
- Team productivity
- Cone of uncertainty
- Agile teams build first
- Agile teams present a range
- Incremental funding

# Keeping track of progress
## Test Monitoring
- Metrics - A set of numbers that give information about a particular process or activity
- Common test metrics
  - Planned work done
  - Test case execution
  - Defect information
  - Coverage
  - Task completion
  - Costs
- Metrics can assess
  - Test approach
  - Quality
  - Progress

## Test Control
- Take control early
- Test Control - Options
  - Re-prioritise tests
  - Change the test schedule
  - Re-evaluate test item entry/exit criterion
  - Add more resources

## Test Reporting
- Types
  - Test progress report
  - Test summary report
- Typical contents
  - Summary of testing performed
  - Information on what occurred during a test period
  - Deviations from plan
  - Status of testing and product quality
  - Factors that block progress
  - Metrics
  - Residual risks
  - Reusable test work products produced
- Progress report
  - Status of testing activities and progress against plan
  - Factors impeding progress
  - Testing planned for the next reporting period
  - Quality of the test object
  - Tailor reports to audience
