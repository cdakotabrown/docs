# QE

## Quality Reporting Dashboard

-   Quality Dashboard
    -   Product(s), applications or services
    -   Tests
        -   Manual (test case)
        -   Automated scripts
        -   Test repository, test count (tracking needed)
            -   Manual
            -   Automatable
            -   Automated
        -   Planned Automation vs Automatable

Create and maintain a quality dashboard to keep track of any relevant products, applications or services. Links to test repositories and boards that track progress on work related to testing. This dashboard should track the team’s test cases alongside metrics on those tests. Metrics include test count by type and code coverage by feature.
Test count is broken down into three categories: Manual, Automatable, and Automated. Manual refers to anything that requires outside intervention to complete, like a user submitting a form or taking a photograph with a device to upload. Automatable and Automated go hand-in-hand to make up the body of automation cases. Automatable tests can are like a to-do list and Automated is anything from that list that has already been completed. The dashboard should have information related to the numbers and ratios between these categories. It’s important to track how many remaining Automatable tasks there are as well as whether there are any Manual tasks that can be promoted into that pile.
Code coverage by feature refers to the amount of automation testing that covers any feature that is added to product or service. Viewers of the dashboard at a glance should be able to see the percentage of completed planned automation, and that amount compared to the whole set of Automatable tests.
What we’re currently using for this: XRay plugins on Jira (<https://jira.walmart.com/projects/WHVCPT?selectedItem=com.xpandit.plugins.xray:testset-panel>)

-   End to End testing resource planning
    -   Refer to master test plan
        -   [Link]
    -   Itemized list of when/where/who we need for e2e testing efforts
        -   Team-internal
            -   Jira stories/planning related to testing
        -   Team-external
            -   Resource names that are accountable to help with testing at certain times
-   Quality Reviews (test case review, automation review, etc)
    -   Create inventory of all products/services that we will be responsible for testing
    -   For each product, create a plan to fill in gaps in our GAP analysis
    -   GAP Analysis
        -   Are tests created? Where are they?
        -   How do we organize tests?
        -   How frequently are tests run?
        -   Time to execute
        -   Traceability matrix
            -   Feature > Code > Unit Test > QA Test
        -   Automation/Coverage metrics (breakdown by feature, might need working session)
    -   Document details of defects
        -   Severity, age, frequency, churn
            -   How frequently are bugs fixed and remain fixed?
        -   Triage process
            -   TODO:
    -   Frequency of quality reviews (Monthly, quarterly?)
-   Keystone Metrics for APIs/UIs
    -   APIs
        -   Devs or business requirements should be responsible for defining metrics for API performance
        -   Simple vs. Typical vs Complex APIs
        -   Unit/Integration tests should be helping to enforce these standards
        -   Make use of performance testing team to better test
    -   UIs
        -   Accessibility
        -   Performance (time-to-paint, first meaningful paint, etc)
-   How does our build pipeline help
    -   Blocking deploys due to integration testing/automation
    -   Blocking merges to main development branch without all unit testing validations passing
    -   Build time tests
        -   Jest/RTL
        -   Running Wyvern stuff against PR deploys
            -   TODO: Workflow diagram
    -   Deploy time tests
        -   Wyvern stuff
-   Testathons
    -   Tester Resources
        -   Applause
            -   Accessibility
            -   Usability/Functional
            -   Certified testers
    -   Non-Tester Resources
        -   User acceptance testing

Training program on how to create unit tests

————————————————————————————————————————————————————————

TODOs for my consumption:
Shree, Bhavin, Rahim, Barry, Neyaz, Jerry, + Any team manager related to this product/service

-   Testing report weekly
    -   Executive summary with details at bottom. Audience is mgmt.
    -   Link to dashboard(s)
    -   [Highlights]
        -   Product/Applications
        -   Features/Team deliverables
        -   Team member kudos
    -   Warning/Heads up
    -   Trend lines/charts/graphics
    -   [Snapshot of dashboard, updates on automation (coverage/cycles run/defects)]
    -
