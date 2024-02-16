# Bugs-Reports

Below are some Bug Report samples that I wrote while working on previous projects.

------------

**OpenWeatherMap API "lang" parameter issue**

**Priority and Severity**

P4 - Low

**Description**

During API testing with Postman on OpenWeatherMap, I found an issue related to the “lang” parameter. It seems that the parameter has incomplete responses from the OpenWeatherMap API.

**Steps to reproduce**

1. Open Postman and create a new Blank Collection by clicking the '+' sign located at the top left corner.
2. Name it OpenWeatherMap.
3. Inside in this collection, click on the blue link “Add a request”.
4. Name it “lang” parameter issue.
5. Paste this link into the URL field “https://api.openweathermap.org/data/2.5/weather?appid=0500095de3678777c748b3b7e230e37f&units=metric&q=Constanta&lang=ro”.
6. Click on the “Send” button.
7. Observe the response in the JSON format.

**Expected result**

The values that are non-numeric and highlighted in orange should be translated into Romanian

**Actual result**

We receive the translation in Romanian only for the “description” and “name” keys, with the correct Romanian translation values. For example, the value for the “main” key remains in English.

**Test data**

I used the following parameters after the “https://api.openweathermap.org/data/2.5/weather?”   endpoint:
”appid=0500095de3678777c748b3b7e230e37f”
”units=metric”
”q=Constanta”
”lang=ro”

------------

**Login is not working properly**

**Priority and Severity**

P2 - High

**Description**

When trying to login with the correct credentials, nothing happens. The user is not logged in and no error message is displayed.

**Steps to reproduce**

1. Go to www.website.com/login
2. Add a correct user / pass

**Expected result**

User should be able to login and is taken to his profile page.

**Actual result**

User is not logged and and no error appears.

**Test data**

User: paul  &  Pass: paul123456

-------------

**Loggin with admin credentials**

**Priority and Severity**

P1 - High

**Description**

When I try to log in with admin credentials, the website shows that I am logged into the account.

**Steps to reproduce**

1. Go to STORE (demoblaze.com).
2. Click on the ‘Log In' link in the top right.
3. Insert in the user and password field the keyword 'admin’

**Expected result**

This account should not be exsit
An error should be displayed with a message ‘Invalid username and password’. 

**Actual result**

This account should not be accessed by everyone. The password and username needed to be changed to another one.
The page shows that I am logged into the account.

**Test data**

User admin & Pass: admin


-------------

**Missing "Forgot Password" Functionality**

**Priority and Severity**

P3 - Normal

**Description**

The "Forgot Password" functionality is absent. Users can't recover their accounts in case of forgotten passwords.

**Steps to reproduce**

1. Go to STORE (demoblaze.com).
2. Click on the “log in” link in the top right corner.
3. Observe that there is no "Forgot Password" link or option

**Expected result**

A "Forgot Password" link or button should be present on the login form, allowing users to initiate the password recovery process. 

**Actual result**

No "Forgot Password" functionality is available, leaving users without recover their accounts in case of forgotten passwords.

**Test data**

User paulp1 & Pass: paulp12

-------------

**Sign Up without confirmation**

**Priority and Severity**

P2 - Normal

**Description**

Users are able to sign up without the requirement of email confirmation.

**Steps to reproduce**

1. Go to STORE (demoblaze.com).
2. Click on the ‘Sign Up' link in the top right corner
3. Create a new account with a new username and password and press sign up.
4. Log in by clicking on the 'Log In' link in the top right corner with the new account.

**Expected result**

Users should be able to confirm their email before the sign-up process is considered complete.

**Actual result**

Users can create a new account without providing an email for confirmation. After clicking the sign-up button, a message is displayed, indicating that the account has been successfully created. Users can log in to the new account without email confirmation process.

**Test data**

User paulp1 & Pass: paulp12


------------

**Missing User Details Page**

**Priority and Severity**

P4 - Low

**Description**

The user details page is missing or inaccessible. There is no link to access the user's personal page.

**Steps to reproduce**

1. Go to STORE (demoblaze.com).
2. Looking for a link to access the user’s personal page, but it is missing.
3. Trying to click on the link ‘Welcome paulp1’ but nothing happens.

**Expected result**

Users should be able to find a link to access the user's personal details page, allowing them to view and edit relevant information, or they should be able to delete the account from this page.

**Actual result**

The link/button to access the user's personal details page is missing.

**Test data**

User paulp1 & Pass: paulp12

------------

**Inconsistent Title and Description for Products**

**Priority and Severity**

P4 - Normal

**Description**

The site displays inconsistent information for product titles and descriptions, causing confusion for users.

**Steps to reproduce**

1. Go to STORE (demoblaze.com).
2. Find the Iphone 6 32gb on the homepage or click here: https://www.demoblaze.com/prod.html?idp_=5
3. Observe the difference between title and description
4.Find the Apple monitor 24 on the next page or click here: https://www.demoblaze.com/prod.html?idp_=10  
5. Observe the difference between title and description

**Expected result**

The product titles and descriptions should match, providing users with clear and reliable information.

**Actual result**

The title is "iPhone 6 32GB," but the description shows "16GB”
The title is “Apple monitor 24” but the description shows “27”

**Test data**

Iphone 6 32gb and Apple monitor 24

-------------

**Application crash on clicking the SAVE button while creating a new user**

**Description**

Application crash on clicking the SAVE button while creating a new the user, hence unable to create a new user in the application.

**Steps to reproduce**

1. Login into the Application
2. Navigate to the Users Menu > New User
3. Filled all the user information fields
4. Clicked on the ‘Save’ button
5. Seen an error page “ORA1090 Exception: Insert values Error…”
6. See the attached logs for more information (Attach more logs related to bug..IF any)
7. And also see the attached screenshot of the error page.

**Expected Result**

On clicking SAVE button, should be prompted to a success message “New User has been created successfully”.

**Actual Result**

After clicking SAVE the application crashes.
