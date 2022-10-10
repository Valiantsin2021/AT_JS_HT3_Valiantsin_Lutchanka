# JS automation API tests using Postman CI integration (Jenkins, Github Actions)

## This repository purpose is to perform API positive and negative test automation of DropBox upload, check metadata and delete file features https://www.dropbox.com/ and perform CI integration of tests with Jenkins and Github Actions

The Dropbox account under the test is created for the testing purposes only and is not a private or personal. Authorization credentials provided in tests are for learning purposes only and to provide the possibility to check the automation task accomplishment.

## Technology used

- Postman (Newman)

## The test suites purpose is to perform the following scenarios:

##### 1. Retrieve the OAuth 2.0 token for authorizing API requests and check user and app authorization
##### 2. Upload the test text file (text.txt) on the Dropbox and check if it is uploaded successfully
##### 3. Check if the uploaded file Metadata is correct
##### 4. Delete the uploaded file (text.txt) and check if it is deleted successfully
##### 5. Perform negative tests for upload, search and delete requests with assertions on wrong endpoints and wrong body/headers data

## Job done:
    
### Postman

1.  Environment with variables and constants
2.  Positive and Negative test suites
3.  Html and junit reporters
4.  Jenkinsfile
5.  Github Actions yml file
6.  Html report publish on gh-pages
7.  Response json schema validation for upload, check metadata and delete file scenarios.
8.  Pre-request scripts for shared tests for various test cases to save in environmental variables
9.  Add Jenkins_local_host_log with job results on the local machine

## Setup:

### Postman tests

1. Clone master branch of this repository
2. Navigate to the folder of cloned repository and run terminal 
3. Install dependencies with "npm install"
4. To run tests - "npm test"
5. To integrate with Jenkins - create new Pipeline and choose Pipeline definition "Pipeline script from CSM", repository url "https://github.com/Valiantsin2021/AT_JS_HT3_Valiantsin_Lutchanka.git", branch "master", Script Path "Jenkinsfile"