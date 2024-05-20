# KapitalSolutionTechAssesment
Technical Assessment for QA Tester
Sauce Demo: - Login Page Automation Test Cases by Cypress.

Documentation:
Test Suite:
describe('Testing Website', () => { ... }): Defines a test suite named "Testing Website" which contains multiple test cases.
Setup:
beforeEach(() => { ... }): Runs before each test case to navigate to the Sauce Demo website.
Test Cases:
 Test Case 1: Login with Valid Credentials:
Steps to input valid username and password and verify successful login by checking the URL.
Test Case 2: Login with Invalid Credentials:
Steps to input invalid username and password and verify the error message.
Test Case 3: Add Product to Cart:
Steps to log in, add the product to the cart, and verify the product is added by checking the cart badge.
Test Case 4. Remove Product from Cart:
Steps to log in, add a product to the cart, navigate to the cart, remove the product, and verify the product is removed by checking the cart badge.
 Test Case 5: Complete Checkout Process:
Steps to log in, add a product to the cart, navigate to the cart, proceed to checkout, fill out the checkout form, and verify the checkout is completed by checking the URL.
Notes:-
1. Tools and Frameworks Used
- *Cypress*: Chosen for its powerful and easy-to-use testing capabilities for web applications.
 2. Test Cases Implemented
•	*Login Functionality*: Verified that users can log in with valid credentials.
•	*Navigation Bar*: Ensured all navigation links direct to the correct pages.
•	*Form Submission*: Tested form submission with both valid and invalid inputs to ensure proper validation and error messages.
3. Challenges and Solutions
- *Error Handling*: Faced issues with asynchronous operations causing tests to fail intermittently. This was resolved by implementing proper wait strategies and retry logic.
- *Coding Intricacies*: Struggled with specific syntax and structure in Cypress. Resolved by consulting the official Cypress documentation and related tutorials.
- *Data Inconsistencies*: Managed test data through fixtures to ensure consistency across tests.

# API Testing
API tests to validate user creation, user update, and data retrieval
operations for Reqres (reqres.in).

 Documentation
Test Case 1: Create user (Test case verifies if a user can log in with valid data.)

Request: Sends a POST request with a username and password.
Response: This JSON response includes a unique identifier and an authentication token likely used to authenticate and authorize a user or session in an API.
Post-response Script: This test checks if the response status code is 200, which means the request was successful and if the response contains two properties: id and token.

Test Case 2:  Create user (Test case verifies if a user can log in with invalid data.)
Request: Sends a POST request with a username and password
Response: The error message {"error": "Note: Only defined users succeed registration"} indicates that only specific, predefined users can successfully register with the Reqres API. Attempts to register any other users will result in this error.
Post-response Script: This CODE includes two tests: one confirms the response status is 400, and the other checks the response JSON contains the error message "Note: Only defined users succeed registration".
Test Case 3:  Retrieve user (Test case verifies to Retrieve User Details.)
Request: Make a GET request to retrieve user details from the API.
Response: Allows easy access to user details and provides metadata for pagination, aiding in the navigation of large datasets.
Post-response Script: The script performs multiple tests on the API response to ensure data integrity, response performance, and correctness of the payload structure. 

Test Case 4:  Update user (Test case verifies to update user information)
Request: Sends a PUT request to update user information
Response: Updated user information via PUT request, ensuring status code 200.Confirmed the updated user details match expected values post-update using a subsequent GET request
Post-response Script: 
The script initially verifies if the response status code is 200, indicating a successful update, and then compares the response data with the data sent in the request to confirm the update. 
Notes: 

#Tools and Frameworks Used
- *Postman*: Utilized for manual API testing and scripting automated tests.
# Test Cases Implemented
1. *GET Endpoints*: Verified that data is retrieved correctly and response times are within acceptable limits.
2. *POST Endpoints*: Ensured data is submitted correctly, with proper status codes and response messages.
3. *Error Responses*: Tested API responses for various error conditions, ensuring appropriate error messages and status codes are returned.
# Challenges and Solutions
- *Understanding API Automation*: Initial unfamiliarity with automated API testing tools. Overcame this by following comprehensive tutorials and participating in online forums.
- *Handling Response Data*: Faced difficulties in parsing and validating complex JSON responses








