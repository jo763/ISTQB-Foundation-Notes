# Understanding SDLC Models
- SDLC: A systematic plan that defines a process and the what? who? when? and how? to deliver software in an organised and efficient way
  - Offers a basis for project planning and control
  - Helps every team player know their role
  - Ensures smooth progress
  - Increases development speed
  - Keeps costs low
- ISTQB SDLC: A model that describes the types of activity performed at each stage in a software development project, and how the activates relate to one another logically and chronologically.
- SDLC Models
  - Sequential
    - Waterfall
    - V-Model
  - Iterative
    - RUP (Rational Unified Process)
    - Scrum
    - Kanban
    - Spiral
- SDLC Stages
  - Analysis
  - Design
  - Development
  - Testing
  - Deployment/Delivery
  - Maintenance
- Waterfall Disadvantages
  - Can be slow and inefficient
  - People wait for others to finish
  - Any phase can become a bottleneck
  - (Very) late feedback
  - Additional pressure on testers
- V-Model
  - Analysis: Acceptance testing
  - System design: System testing
  - High-level design: Integration testing
  - Low-level design: Unit testing
- Models are a simplification of reality
- Iterative models are NOT always better than sequential
  - Context matters
  - A robust sequential model may be good enough
  - Mixing models is possible in practice

# Discovering Test Levels
- Four levels
  - Component
  - Integration
  - System
  - Acceptance
- Common Objectives
  - Reducing risk
  - Verifying functional and non-functional behaviours
  - Build confidence in the system
  - Find defects
  - Prevent defects from escaping to higher levels

## Component Test Level
- Component testing (aka unit or module testing) focuses on components that are separately testable

## Integration Test Level
- Testing 2,3,4 (more than 1 unit) etc together. is  integration testing
- Test objects:
  - subsystems
  - Databases
  - Infra components
  - Microservices
- Test basis:
  - Tech spec
  - Design docs
  - Sequence diagrams
  - Public interface definitions

## System Test Level
- Full integration testing of all modules
- Starting point is outside system
- Consider system's paths and flows

## Acceptance Test Level
- Important to have clear and complete requirements
- User acceptance testing (UAT)
- Operation Acceptance Testing
  - Backup and restore
  - Installing, uninstalling, upgrading
  - DR
  - Data load and migration
  - Performance and load testing
- Alpha and Beta testing
  - Beta testing: for commercial off-the-shelf (COTS) software
  - Both  carried out by independent testers and potential customers
  - Alpha testing happens at the developer's testing
  - Beta testing happens at the site of the customer
  - The point of Beta testing is to use the infrastructure, both of the hardware and the software, of the end users.

# Comparing Test Types
- Test type: A group of test activates aimed at testing specific characteristics of a software system
- Two main groups
  - Functional
  - Non-functional

## Functional Testing
- Does the feature function correctly? as expected?
- Types:
  - Unit (or module)
  - Integration
  - System - UAT
  - User Interface (UI) - UAT
- Coverage: The degree to which an application is exercised by tests expressed as a percentage
- Coverage gap: Percentage of tests not exercised as a percentage

## Non-Functional Testing
- Answers How well? How fast? How stable? How usable? how secure?
- Types:
  - Usability
  - Performance
  - Security
- Usability:
  - More than just "make text on button bigger"
  - May be achieved via alpha and beta testing
- Performance:
  - Specialist area
  - types:
    - Stress
    - Load
    - Endurance
    - Spike
    - Scalability
- Security:
  - Huge domain
  - AKA: Penetration testing, ethical hacking, white-hat hacking
  - Separate career path: Course on pluralsight

## Change-related Testing
- Confirmation testing: Was the bug really fixed?
- Regression Testing: Did the fix (or the change) break anything else?
- Regression: Any unintended side-effect caused by a change, can cause a regression bug from a fix
- Test automation can run x100+ faster and prevents testing from becoming a bottleneck
- Change types:
  - Bug fix
  - New features
  - Change to existing features
  - Configuration and environmental changes

## Test Types and Test Levels
- ISTQB: You can do any test type at any test level (in reality this has rare combinations and some are not meaningful)
- Black-box is typically carried out at higher levels e.g. acceptance and system
- White-box pretty much means unit testing
- Grey-box testing is integration as it's a mix

# Understanding Maintenance Testing
- Systems need to be maintained because changes are inevitable
- Two categories
  - Unplanned
    - Bugs or failure in production
    - A "hotfix" required
  - Planned:
    - Software enhancements
    - Operational and environmental upgrades
      - E.g. SQL server to a newer version
    - Retirement of a system
      - Software may not be fit for purpose anymore
      - Typically means rewriting the software using newer tech
- Impact Analysis: Evaluates the changes made to identify consequences and potential side-effects
  - What has changed?
  - Where in the system?
  - Which parts are definitely affected?
  - Which parts are likely to be affected?
- Challenges:
  - Outdated specifications
  - Lack of knowledge
  - Outdated test cases with no traceability
  - Weak or non-existent tool support
