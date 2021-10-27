# ww-automation-code-test
In this test you will find a wide cross section of the type of code you will be exposed to at Wealth Wizards.

Most candidates complete the test in under 3 hours, however if you should wish to continue beyond that we welcome you to do so and this will have no impact on your submission.

## Instructions
Click the **Use this template** button above to create a private repository in your own github account and invite github user @Tom-Hudson as _collaborators_ on your repo.

**IMPORTANT: Please commit your work on a new branch and raise a pull request against the master branch of your repo and add us as reviewers. Please add a simple description to your PR outlining which parts of the test have been completed and any comments you feel support your submission.**
 
* You have all the flexibility you want to create the test project: It’s up to you how you design the scenario(s), if you want to split it in multiple tests, if you want to use specific npm packages etc. 

* Please complete as many parts of the test as you can, we recommend you complete them in order. Add a description to your PR outlining which parts of the test have been completed and any comments you feel necessary.


### Part 1: Create a JS npm project with cypress.io 
Use Cypress.io to automate the below scenario under `cypress/integration/part1-Tests` directory:
1. Go to https://www.wealthwizards.com/  
2. Check that About Us dropdown has 3 values: “Who we are”, “Careers” and “Contact”
3. Click on “Careers” - you should get redirected to https://www.wealthwizards.com/careers 
4. Check the 5 WW values
5. Check that the page contains “View jobs” button
6. Click “View jobs” button   - you should get redirected to https://www.wealthwizards.com/job-vacancies  
7. Find a role  and click “Find out more” button
8. Validate the page 

### Part 2: Test Reporting
Add functionality to create a html report from your cypress test run under `report-html` directory.

### Part 3: Visual test
Integrate with a Visual testing tool (Percy/Applitools) to validate the Lead Quality Engineer role page 

* You can register for a free account for Percy (https://percy.io/ ) or Applitools (https://applitools.com/ ). 
* Run the test against  2 browsers (Chrome & Edge) and 3 different resolutions (mobile/tablet and desktop).
* Take full page screenshot from Percy/Applitools and add it into `part3-VisualTest` directory.

### Part 4: CI Integration 
How would be integrate your tests to run into CI - could you draft a **Jenkinsfile**? Or another CI pipeline that can be integrated with your Github project? 
* Note: We use Jenkins as our CI tool and that’s the reason we started with Jenkinsfile, but feel free to use any other available option to integrate your project into a CI tool. 
* We understand you might not be able to validate the CI pipeline, but even a draft would give us an idea over your CI understanding. 
* Where you don't know the Jenkins/Groovy technical format, it’s sufficient to add a comment and explain your intention for that step
* Add the file into `part4-CI` directory.

### Part 5: Cucumber 
Create a Cucumber Feature file to test 2021 income tax rules for UK (https://www.gov.uk/income-tax-rates ).  
* Gherkin Reference - Cucumber Documentation: https://cucumber.io/docs/gherkin/reference/   
* Note! We understand the project won’t have the step definitions for the feature file to work, we are only interested into how the scenarios are created at this point.
	* Tests to be created for a single individual eligible for income tax and Personal Allowance 
	* Savings / Dividends to be ignored. Only taxable income to be considered.
