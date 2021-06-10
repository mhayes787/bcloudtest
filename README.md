# bcloudtest

Welcome to the bcloudtest project! Using the Page Object Model (POM), the purpose of this application is to automate the steps listed below using the Cypress test automation tool. 

1. Navigate to www.bettercloud.com

2. Locate and click on "Company" in the navigation bar

3. Check that "About BetterCloud" is visible as H1

4. Locate and click the "Board" tab in the navigation bar on teh page

5. Locate and extract the name and excerpts from the profile cards of all board members into a CSV spreadsheet

6. Save the CSV file in a dedicated folder of the root directory of your code, named 'export'.

### Bonus steps

1. Use your desired automated solution to save snapshots, videos, or report results of your test

2. Setup a CI environment to run your automated test. 

## How to access the Cypress bcloud test automation tool

1. In your web browser, go to www.github.com

2. Log into your Github account and enter your credentials
   **Note:** If you do not have an account, please feel free to create one

3. In the search field, input the following "mhayes787/bcloudtest" and press "Enter or Return" on your keyboard

4. At this point, you should be able to view the project. Click on the green button that says "Code, Clone, or Download"

5. Copy the URL (https://github.com/mhayes787/bcloudtest.git) and clone the repo to a local directory on your laptop or desktop

6. Once step 5 is complete, access the project locally, via command line by running the following commmand "cd bcloudtest"

7. Last, run the following command "npm install"

## Prerequisite to test bcloudtest tool

1. Need to have node.js installed on your system
   * If node.js is already installed on your system, you should be able to install packages via npm command
   * If node.js is not installed on your system, go to the node.js website (https://nodejs.org/en/download/) to download

2. Need to have Cypress intalled

## How to install Cypress via npm

* From your project directory, run the following command "npm install cypress -save-dev"
  **Note:** This will install Cypress locally as a dev dependency for your project

## How to install Cypress via yarn

* From your project directory, run the following command "yarn add cypress -dev"

## How to Test bcloud automation tool based on steps mentioned above

### Option 1

1. From your terminal, run the following commands:
   * cd node_modules (press "Enter or Return" on keyboard)
   * cd cypress-page-object-model (press "Enter or Return" on keyboard)
   * Type "npx cypress open" (press "Enter or Return" on keyboard)
     **Note:** This opens the Cypress Test Runner, which includes the following options "Tests, Runs, and Settings".
     
2. From Cypress Test Runner, click on "Tests"

3. Click on the following file "bcHomePage.spec.js"
   **Note:** The browswer will appear and you should see the test suites and test cases, along with the automation appearing on the right.

### Option 2

1. From the terminal, run the following command "npx cypress run" (press "Enter or Return" on keyboard). This command runs all the tests headlessly and a report is generated in the terminal, which tells your how many tests passed and/or failed 
**Notes:** Make sure your are in the following directory "betterCloudTest/node_modules/cypress-page-object-model" before runnng the command. Also, you should see the "export.csv" file in the root directory with both options

### Option 3 (Record and view test results)

1. From terminal, run the following command "npx cypress run --record --key 54d1f1c9-b8ab-4a30-81ae-8e986a2a2b36" (press "Enter or Return" on keyboard)

2. Similar to option 2, this command runs in headless mode and a report is generated in the termianl and Cypress Dashboard

3. From the terminal, open the Cypress Test Runner (npx cypress open)

4. Click on the "Runs" tab and you will see some results
   **Note:** It may ask you to "Log In to Dashboard" before viewing the results. You may have to create an account

5. Click on your result and you will be able to see a summary overview of your results

6. Click on the "Test Results" tab 
   **Note:** You should be able to see the "bcHomePage.spec.js" file, along with each test
 
7. Click on one of the test
   **Note:** An aside menu should a appear and give you the option to watch the video. Also there are other options such as Runtime environment, Artifacts, Test code history, etc...



