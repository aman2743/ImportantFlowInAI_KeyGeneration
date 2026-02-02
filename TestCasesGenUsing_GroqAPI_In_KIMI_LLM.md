1. Launch Terminal
2. Change the directory where project Exits in VScode
     $ cd "D:\VScodeProject\TestCaseGenUsingGroqAPI"
3. Now type kimi next to Project Directory
4. Now Type /login
5. Select first option and it should naviagte user to login and make sure user is login successfully
6. Prompt to create test case Generator  
promode@TestCaseGenUsingGroq Can you please create a test case generator where the user will type a query and you will be generating a test case? And all you have to do is you have to use the API of GROQ. I am going to share the Groq API key with you. It is GROQ. Please remember that. And you have to basically create a UI for that. Okay? With me?

<img width="1723" height="945" alt="image" src="https://github.com/user-attachments/assets/7ce6da39-df3a-449c-bcb5-edf962841f4f" />


I was able to create the test cases successfully after providing the key
Here are 10 comprehensive test cases for the login page:

- Test Case ID: TC001
- Title: Valid Login Credentials
- Precondition: User has a valid username and password
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a valid username
  3. Enter a valid password
  4. Click the login button
- Expected Result: The user is successfully logged in and redirected to the dashboard
- Priority: High
- Type: Positive

- Test Case ID: TC002
- Title: Invalid Username
- Precondition: User has an invalid username and a valid password
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter an invalid username
  3. Enter a valid password
  4. Click the login button
- Expected Result: An error message is displayed indicating that the username is invalid
- Priority: Medium
- Type: Negative

- Test Case ID: TC003
- Title: Invalid Password
- Precondition: User has a valid username and an invalid password
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a valid username
  3. Enter an invalid password
  4. Click the login button
- Expected Result: An error message is displayed indicating that the password is invalid
- Priority: Medium
- Type: Negative

- Test Case ID: TC004
- Title: Empty Username Field
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Leave the username field empty
  3. Enter a valid password
  4. Click the login button
- Expected Result: An error message is displayed indicating that the username field is required
- Priority: Medium
- Type: Negative

- Test Case ID: TC005
- Title: Empty Password Field
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a valid username
  3. Leave the password field empty
  4. Click the login button
- Expected Result: An error message is displayed indicating that the password field is required
- Priority: Medium
- Type: Negative

- Test Case ID: TC006
- Title: SQL Injection Attempt
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a username with a SQL injection attempt (e.g. `OR 1=1`)
  3. Enter a valid password
  4. Click the login button
- Expected Result: The application prevents the SQL injection attempt and displays an error message
- Priority: High
- Type: Negative

- Test Case ID: TC007
- Title: Password Length Validation
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a valid username
  3. Enter a password that is less than the minimum required length
  4. Click the login button
- Expected Result: An error message is displayed indicating that the password length is invalid
- Priority: Medium
- Type: Boundary

- Test Case ID: TC008
- Title: Maximum Login Attempts
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter an invalid username and password
  3. Repeat step 2 for the maximum number of allowed login attempts
  4. Click the login button after the maximum attempts
- Expected Result: The application locks out the user after the maximum number of allowed login attempts
- Priority: Medium
- Type: Boundary

- Test Case ID: TC009
- Title: Forgot Password Functionality
- Precondition: User has a valid username
- Steps:
  1. Launch the application and navigate to the login page
  2. Click the forgot password link
  3. Enter a valid username
  4. Click the reset password button
- Expected Result: A password reset email is sent to the user's registered email address
- Priority: Medium
- Type: Positive

- Test Case ID: TC010
- Title: Cancel Login
- Precondition: None
- Steps:
  1. Launch the application and navigate to the login page
  2. Enter a valid username and password
  3. Click the cancel button
- Expected Result: The login process is cancelled and the user is redirected back to the login page
- Priority: Low
- Type: Positive
