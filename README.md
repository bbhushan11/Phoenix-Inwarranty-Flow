# Postman API Automation Integratio with GitHub Actions #

This repository is a demonstration for POC for integrating Postman tests with Github Actions. The test are written in Postman and they are executed on the Virtual Machine with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main branch. You can also execute the project manually using workflow_dispatch. The projects run on a scheduled time with the help of CRON job.

The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from the github page : https://bbhushan11.github.io/Phoenix-Inwarranty-Flow/
The latest report is mailed to the team members using GMAIL SMTP.

## About Me ##
Hello, My name is Bhushan Pathak. I have 4+ years of experience in Automation Testing and DevOps. My Skillset includes UI Automation with Selenium Webdriver with Java, Webdriver IO, Playwright with Java Script and for API testing I use Postman.
You can connect with me over : https://www.linkedin.com/in/bhushanpathak11/

## Testing Coverage ##
1. Positive Test Cases Coverage
2. Negatibe Testing and Edge Case Testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation

## Tech Stack ##
1. Postman
2. Node.js 22v
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. GMAIL SMTP
7. Github pages
8. CSV for Data Driven Testing

## Github Pages ##
You can directly view the latest test report of the Postman Test at the Github Page Link : https://bbhushan11.github.io/Phoenix-Inwarranty-Flow/

## HTML Report ##
The report will be created in the newman folder 
![Postman report](https://github.com/bbhushan11/Phoenix-Inwarranty-Flow/blob/static-content/Newman-report.png)

## Project Structure ##

```
Phoenix Inwarranty Flow
├─ Inwarranty-flow Collection Copy.postman_collection.json    # Collection File
├─ QA.postman_environment.json    # Environmental File
└─ testData.csv     # TestData File     

```

## How to run the Project? ##
You can run the Project on your local system for that:
1. Clone the project on Local System : https://github.com/bbhushan11/Phoenix-Inwarranty-Flow.git
2. Install Node.js and NPM from https://nodejs.org/en
3. Install Newman using ```npm install -g newman```
4. Install Newman-reporter-htmlextra using ```npm install -g newman-reporter-htmlextra```
5. Run the Newman command :
   ```
               newman run 'Inwarranty-flow Collection Copy.postman_collection.json' \     
              -e QA.postman_environment.json \
              -d testData.csv \
              -r cli,htmlextra \
              --reporter-htmlextra-export ./newman/index.html
   ```

   
   

