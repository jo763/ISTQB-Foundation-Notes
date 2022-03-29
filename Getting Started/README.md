# Topics covered by Foundation
- Fundamentals of Testing
- Testing throughout the SDLC
- Testing techniques
- Static testing
- Test management
- Tool support for testing

# What is Testing
- Test planning: What, how, by when?
- Analysis
- Test design
- Test execution and checking the results
- Bug reporting
- Test reporting

## Testing Objectives
1. To PREVENT defects by evaluating work products such as requirements, user stories, design and code
 - An example may include testing the design so the product isn't built to a bad spec
2. To find defects and failures thus reduce the level of risk of inadequate software quality
  - Reviewing and evaluation requirements is preventing (best)
  - Finding bugs in built software is reacting (second best)
3. To verify whether all specified requirements have been fulfilled
4. To check whether the test object is complete and validate if it works as the users and other stakeholders expect
5. To build confidence in the level of quality of the test object
6. To provide sufficient information to stakeholders to allow them to make informed decisions
7. To comply with contractual, legal or regulatory requirements of standards
- Testing is not debugging.
  - Executing tests can show failures that are caused by defects in the software
  - Debugging is something that is carried out by developers to find and fix the underlying cause
  - Testing is finding issues and confirming fixes
  - Debugging is finding and fixing the root cause

## Why is Testing Necessary?
- Mistakes can be very costly (and potentially deadly)
- High quality has a price, but low quality can be more expensive

- Testers can and should:
  - Be involved in the review of requirements
  - Participate during design - increasing each party's understanding
  - Work closely with developers and system designers
  - Verify and validate the software prior to release
### Quality Management (QM)
- Quality Assurance (QA)
  - Adherence to process - Are we doing things according to the established process?
  - Managing tool, proactive, prevents defects
- Quality Assurance (QA)
  - Various activities including:
    - Testing
    - Test design
    - Test execution
  - Reactive, detect bugs
- Hierarchy
  - QM
    - QA
      - QC
        - Testing

### Error, Defect, Failure
- Error: Mistake
  - e.g. BA misunderstood the client
  - e.g. Developer misunderstood the requirements
- Defect: Bug (N.B. tends to be used by everyone in industry to refer to mistake,, defect or failure)
  - Caused by errors
  - A mistake built into the software
  - May or may not lead to failure
- Failure
  - Bug that manifests itself while using the software

### Why do mistakes happen?
- Time pressure
- Human fallibility
- Inexperience and lack of skill
- Complexity
- Misunderstandings
- New and unfamiliar tech

- Potential causes of failures
  - Poor unreviewed requirements
  - Bug fixes creating more bugs
  - Verifying things without enough information or skill
  - Is there little communication between the stakeholders
- ROUTE CAUSE ANALYSIS SHOULD NOT BECOME BLAME GAME but opportunity to improve instead

# Seven Testing Principles
1. Testing shows the presence of defects not their absence
2. Exhaustive testing is impossible
3. Early testing saves time and money
4. Defects cluster together
5. Beware of the Pesticide Paradox
6. Testing is context dependent
7. Absence of errors is a fallacy

## 1. Testing shows the presence of defects not their absence
- Absence of evidence is not evidence of absence
- Never say:
  - This software has no bugs
  - This system is completely bug free
- Can create incorrect and dangerous expectations
- Say instead:
  - I haven't found any (more) bugs
  - I haven't found any further issues
- Sets more accurate expectations

## 2. Exhaustive testing is impossible
- Possible only in most trivial cases
- Not possible in non-trivial cases due to infinite no. options
- Exhaustive testing alternative
  - Select a portion
  - Test portion
  - Assume rest is ok
- Selecting combinations (portion)
 - Risk analysis
 - Test techniques
 - Contextual priorities

## 3. Early testing saves time and money
 - Earlier you notice a problem, the better

## 4. Defects cluster together
- Typically small case of modules have most of the defects
- Useful for when you don't have lots of time to test

## 5. Beware of the Pesticide Paradox
- Tests initially catch bugs, with time the same tests stop catching anything
- To detect new defects
  - Review and change existing tests and test data
  - create new tests
- Defining tests with a bit of flexibility, say test with extremely large number over 11 digits instead of 11 billion for a number input

## 6. Testing is context dependent
- Your priorities, testing approach and entire workflow will be affected by your surroundings

## 7. Absence of errors is a fallacy
- Fallacy: A false or mistaken belief. It is something that might appear true, but in reality, it's not.
  - e.g. If we find and fix a large number of defects, then we can be sure that our software is of high quality
- Even if you catch and fix many defects, you're not guaranteed success

# Test Process Fundamentals
## Context
- External stakeholder interests
- Domain
- Law and Standards
- SDLC (e.g. Agile vs waterfall)
- Budget, resources and time
- System complexity

## Test Activities and Tasks
- Test activities
  - Test planning
  - Test monitoring and control
  - Test analysis
  - Test design
  - Test implementation
  - Test execution
  - Test completion

## Test Planning, Monitoring and Control
### Test Planning
- Defining objectives of testing
- Specifying how you are going to achieve those objectives
  - Test techniques
  - Schedule and deadlines
- Test plan can be (and often is) adjusted during testing

### Monitoring and Control
- On-going comparison of planned vs actual
  - Are we doing what we planned to do?
  - Are we on track?
  - Should we communicate our findings already? (Yes)

## Test Analysis
- Better understanding of the system leads to better tests
- Analyse anything you can get your hands on (test basis)
  - Requirements
    - Business
    - Functional
    - Non-functional
  - Design
    - Architecture diagrams
    - UML diagrams
    - Anything else created by technical people who designed the system
  - Code
    - Code
    - Metadata
    - Dev documentation
    - System interface documentation
  - Risk analysis reports (if existing)
- Looking at test basis products
- Identifying all possible defects
  - Ambiguities
  - Omissions
  - Inconsistencies
  - Inaccuracies
  - Contradictions
  - Superfluous statements

## Test Design
- Designing and prioritising tests
- Identifying necessary test data
- Preparing the test environment
- Capturing bi-directional traceability between the test basis, test conditions and test cases
- Test design is how to test, terst implementation is do we have everything in place to run the tests
- Test Implementation
  - Developing test procedures and automated test scripts (if applicable)
  - Setting up the test environment
  - Preparing test data
  - Verifying and updating traceability

## Test Execution
- Set things up then execute the tests
- Compare the expected and actual results
- If don't match i.e. unexpected output then analyse and double-check
  - Setup correct?
  - Setup followed faithfully
  - Test scenario makes sense and has no faults?
    - Analysts, developers and testers can make mistakes
  - If still wrong, write bug report
  - Log (report) all test outcomes, pass, fail, skipped, blocked

## Test Completion
- Ensuring that all defect reports are closed
- Creating a test summary report
- Finalising, archiving and (or) sharing testware
- Analysing lessons learnt

## Test Work Products
- Test Planning: Test Plan (what? how?)
- Test Monitoring and Control: Test Progress Reports, Test Summaries
- Test Analysis: Test Conditions, Direct Reports
- Test Condition: A testable aspect of a component or system identified as a basis for testing
- Useful Glossary: https://glossary.istqb.org/en/search/
- Test Design and Implementation: Traceable Test Cases
- Test Execution: Test Status (Pass, fail?, skipped, blocked), bug reports
- Test Completion: Summary reports, improvement action items

# Test Psychology
- Testers must have interpersonal skills
- People can be defensive about bugs, can become blame game, fighting instead of cooperating
- Don't provide overly critical feedback and bug reports
- How not to be the bearer of bad news
  - Establish a relationship with developers
    - You are on the same side
  - Say that you are here to support them
  - Fixing bugs early saves time and stress for everyone
- How not to be the critic
  - Bug reports and communication must be:
    - Constructive
    - Clear
    - Informative
    - Bug report must answer What?, When?, How?
      - Software version tested
      - Link to relevant requirements
      - Short description
      - Concrete steps taken to reproduce the failure
      - Expected result
      - Actual result
      - Screenshots, log snippets or other applicable useful information
      - Cutting corners may save you 1 min but can cost 5+ mins to others
      - Read your own report, no criticism of any kind
      - Only information pertinent to understanding, reproducing and fixing the issue
    - Try and understand the other person, why do they react negatively
    - Confirm common understanding, listen and repeat back

## Tester vs Developer mindset
- Bias: The tendency to favour information that confirms or supports our beliefs and values. Often at the expense of facts
- Mindsets
  - No bugs until proven otherwise (Developer) innocent until proven guilty
  - Always have bugs (Tester) guilty until proven innocent
- Those who build don't want additional work (fixing bugs)
  - Tendency to seek proof that it works fine
- Those who test think the opposite
  - Tendency to always think there's still a bug to be found
- Tester mindset should include
  - Curiosity
  - Professional pessimism
  - Critical eye
  - Attention to detail
  - Motivation for good and positive communications and relationships

# Further Study
- ISTQB
  - CTFL Syllabus 2018 v3.1.1: https://www.istqb.org/certifications/certified-tester-foundation-level

- Out of scope
  - guru99.com/software-testing.html
  - softwaretestinfundamentals.com
