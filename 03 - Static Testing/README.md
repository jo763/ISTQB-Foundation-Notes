# Static Testing Essentials
## Static Testing
- Code is never executed. or run
- Static testing is used EARLY in the SDLC
  - Before something goes wrong
- Manual review techniques
  - Informal reviews
  - Walkthroughs
  - Formal tech reviews
  - Software inspection
- Max benefit from early SDLC reviews
- Tool-based techniques
  - Static analysis is tool-driven evaluation of any work products with structure e.g. code
  - Important for safety critical systems
  - Security testing
  - Static analysis is often incorporated into automated build and delivery systems
- Examples of software work products
  - Business requirements
  - Architecture and design specs
  - Epics, user stories, acceptance criteria
  - Code
  - Web pages
  - User guides
- Static testing techniques examine the software work products early; before something goes wrong

## Benefits
- Defects found early are cheaper to remove
- Production defects can be costly
- Static testing is an investment
- Static testing improves productivity, prevents defects and reduces costs.

## Static vs Dynamic
- Dynamic
  - Test conditions are identified
  - Test cases must be written
  - Test data must be sourced
  - A test environment is required
  - Tests are run against the code
  - Testers observe and report failures
  - External focus

- Static
  - Code does not have to be executed
  - Defects are found in the work products
  - A dormant defect can be identified
    - on a rarely exercised path
    - or it may be hard to reach
  - Internal focus

- Static Defects in Spec
  - Review of requirements will find omissions, inaccuracies, redundancies, inconsistencies, ambiguities and contradictions

- Static Defects in Design
  - Inefficient algorithms
  - Inefficient DB structure
  - High coupling, low cohesion

- Other static defects
  - Deviations from coding standards
  - Incorrect interface specs
  - Security vulnerabilities
  - Gaps in the test coverage
  - Maintainability defects can only be found by static testing

# The Review Process
- Review Process
  - How to plan a review
  - Initiation of a review
  - Individual review (preparation)
  - Issue communication and analysis
  - Fixing and reporting

- Why review?
  - Prevent defect migration
  - Cost of fixing defects increase later in the lifecycle
  - Reviews examine work products early in the lifecycle and raise issues

- An issue can be a potential defect or a recommendation or a questions

- Different characteristics of reviews
  - Informal Review
    - No defined process
    - No formal documented outputs
  - Formal review
    - Team participation
    - Documented results
    - Documented procedures

- Review Types (according to ISTQB)
  - Informal Review
  - Walkthrough
  - Technical review
  - Inspection

## How to plan a review
- What is the purpose of the review? Scope?
- What is to be reviewed?
- Identify quality characteristics

- Planning - review characteristics
  - Review type
  - Activities
  - Roles
  - Checklists

- Estimate effort and timeframe
- Entry and exit criteria
  - Entry criteria must be checked before the review can start
  - Exit criteria must be met before the work product can be approved
- Initiate Review
  - by:
    - Face-to-face workshop
    - Virtual meeting
    - Email
  - Distribute work product
  - Explain the process
  - Answer questions

## How to run a Review
- Individual review
  - Note potential defects
  - Note your questions


- Communicating issues in a review meeting
  - Potential defects
  - Recommendations
  - Questions
  - Analysing potential defects
  - Assinging ownership and status
- Quality characteristics
  - Evaluate any issues raised
  - Document the findings
- Make a decision
  - Accept "as is"
  - Accept with minor changes
  - Reject as major changes required
- 4 aims
  - Communicate defects
  - Assign ownership
  - Evaluate QCs
  - Make a review decision

### Fixing and Reporting
- Create defect reports
- Fix defects
- Communicate defects
- Update defect status
- Gather metrics
- Check exit critera are met
- Accept the work product

- Reviews are static testing techniques used early in the lifescyle to identify potential defects in work products

### Roles and Responsibilites in a Formal Review
- Author
  - Creates the work product
  - Addresses the issues
- Facilitator
  - Runs an effective meeting
  - Mediates different viewpoints
- Scribe
  - Collates issues found earlier
  - Records new issues
- Review Leader
  - Takes overall responsibility
  - Select participants
  - Organises when and where
- Management
  - Responsible for review planning
  - Decides review strategy
  - Assigns staff budget and time
  - Monitors cost effectiveness
  - Executes control decisions
- Reviewers
  - Can be
    - Technical guru
    - Project staff
    - Business expert

- ISO/IEC 20246 - for more detailed explanations of the review process for work products

# Review Types Compared
## Informal Review
  - Purpose: detect defects, generate ideas
  - People: buddy developer
  - Process: none
  - Post-review: limited documentation

## Walkthrough
- Author prepares well
- Aim to improve product
- Author presents the material
- Advantages:
  - No demands on the participants
  - Large audience - diverse viewpoints
  - Important issues likely to be found
- Disadvantages
  - Boredom from some
  - Questions for clarification only
  - Author may get defensive
- A walkthough may involve scenarios, dry runs or simulations
- Purpose: find defects, improve
- People: author led, many participants
- Process: varies from informal to formal
- Post-review: defect logs and reports

## Technical review
- Process:
  1. Planning
  2. Initiation
  3. Individual review (prep)
  4. Issue communication
  5. Fixing and reporting
- Purpose: gain consensus, find defects
- People: peers of the author
- Process: formal, meeting is optional
- Post-review: fixing and reporting

## Inspection
- Defined process
  - Plan
    - Tean roles
    - Entry criteria, rules/guidelines
  - Kick-off
    - Checking rate
    - Perspectives
  - Study
    - Checklists
  - Meet
    - Logging issues
  - Fix
    - Exit criteria

- Purpose: find defects, improve process
- People: small team, assigned roles
- Process: formall, defined
- Post-review: metrics reported

## Review Techniques
- Ad-Hoc
  - Prep is minimal
  - Relies on reviewer expertise
  - No guidance given
  - Work product read sequentially
  - Duplicate issues are common
- Checklist-based
  - Systematic technique
  - Checklists distributed at initiation
  - Typical defect ypes are covered
  - Look outside the checklist
  - Offer advice to reviewers
  - Have a question format
  - Derived from the rules (inspection)
  - One checlist per work product
  - Checklists must be updated
    - When new defects are found
    - When questions are outdated
  - A checklist is one page
- Scenarios
  - Structured guidelines on reading
  - Supports "Dry Runs"
  - Better than simple checklists
  - Don't be constrained
- Role-based
  - Experienced user
  - Senior citizen
  - Child user
  - Novice user
  - Infrequent user
  - Developers/Testers/Performance/Systems Admin
- Perspective-based
  - PBR: Perspective-based reading provides concrete instructions to help you uncover defects
  - Reviewers use stakeholder roles
