# Business-Analysis

# NOTES

<details>
<summary>X1. Epics </summary>

# Epic - Counsellor Onboarding

### Description

As a counsellor i want to be able to onboard on the e-counselling web app so that i can have access to the system.

![image](https://github.com/omeatai/Business-Analysis/assets/32337103/832bcd8b-082f-4d89-a378-4a09060c499c)

<img width="1534" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/33dfd961-b282-4183-8d37-3f7ca3e2f64c">
<img width="1534" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/c2b979f0-6d9b-4c57-8b1b-9e884de15763">
<img width="1534" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/f1373f96-f137-4fde-b31b-009272abcbee">


#END</details>
<details>
<summary>X2. User Stories & Acceptance Criteria </summary>

# User Stories & Acceptance Criteria

### Why do we need this?

- We need to be able to provide users with an interface in the app to sign-in securely by entering their login credentials so that they can be verified and allowed access.

### Job Story

- As a user
- I want to be able to provide my email and password
- So that i can sign-in to have access to the application

### Preconditions

- User must have a valid email address
- User is on the login page of the application

### User Flow

- User opens app and is shown login page if not logged in
- User enters email address
- User enters password
- User clicks on [sign-in] button

### Post conditions

- User credentials are verified.
- If credentials are valid, User is granted access to application’s features.

### Acceptance Criteria

#### On successful Login, existing Users will be granted access to the app. 

- GIVEN that User is existing
- AND Login Page is loaded
- WHEN mandatory fields are correctly populated with credentials
- AND the User clicks on the "Sign-in" button
- THEN the User is verified 
- AND granted access to the application

#### All mandatory fields must be populated correctly to successfully login.

- GIVEN that User is existing
- AND Login Page is loaded
- WHEN mandatory fields are NOT correctly populated with credentials
- AND the User clicks on the "Sign-in" button
- THEN the User's verification will fail 
- AND redirected back to the Login page
- AND an Error message is displayed to confirm failed attempt

#### New users cannot login because verification will fail and will receive an error message on attempt. 

- GIVEN that User is new
- AND Login Page is loaded
- WHEN mandatory fields are correctly populated with credentials
- AND the User clicks on the "Sign-in" button
- THEN the User's verification will fail
- AND redirected back to the Login page
- AND an Error message is displayed to confirm failed attempt  

#### Happy Path

- Must ensure that the email address follows the format of hello@yourmail.com
  
- Must ensure that the password satisfies the following conditions

```txt
- minimum of 6 characters
- maximum of 12 characters
- must be alphanumeric
- must have at least one uppercase
- must have at least one lowercase
- must have at least one number
- must be hidden on the password field with asterisk*
```

- Must ensure that the login page loads in less than one second.

- Must ensure that when the user clicks on the Sign-in button,  that the user’s credentials are immediately sent to the backend for verification when credentials are correctly entered.

#### Unhappy Path

- Must ensure that if the User enters an incorrect email format

```txt
- The error message should say: ‘You have entered a wrong email format. Please ensure your format is hello@yourmail.com’ 
- The error message should appear below the email address in red font colour.
```

- Must ensure that if the User enters the wrong email or password

```txt
- The error message should say: ‘Your email or password is incorrect. Try again!’
- The error message should appear above the email address in red font colour.
```

- Must ensure that “Forgot Password” link option is provided to reset password if user has forgotten the password.

- Account should be locked after 5 failed login attempts.

<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/5f9e75dc-24e5-45ca-a1d8-6feb40828476">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/dea804a4-f03c-4341-8920-c88d3f1267aa">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/9cacb6c7-2cdc-4828-94fc-2af68951b466">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/ad981223-b26e-464b-817a-2b5976253258">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/e81b5d63-72fc-4508-adfc-97fdbbcd31f2">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/fc21249c-0f95-4da4-a4d2-fe4d0c5d8f00">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/9f640d25-d5c9-4eb8-b934-bb3b1eea51a7">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/0519441a-0ee7-4f5c-aaf3-9f2b6cbd1285">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/2ac8423c-fb15-48bb-983b-f5068091874b">
<img width="960" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/3acdcc51-2af2-4d7d-a8df-24ae3f860fa2">

<img width="1534" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/95c7a92c-3e61-4e57-9fcd-70140afcecf8">
<img width="1490" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/b59d2070-b794-4ca0-b843-566c10fdbbe5">
<img width="1534" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/69c1db3d-a4ac-4b69-826c-aa6fdb08cdcb">
<img width="1490" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/0cc7f1b4-3507-4300-a9e1-2941ab396d59">
<img width="1490" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/bb00a818-8dec-49d4-9889-2fb140c8bb20">
<img width="1490" alt="image" src="https://github.com/omeatai/Business-Analysis/assets/32337103/8aeb14c8-a861-4a9d-8ee3-272e88a40379">

#END</details>
<details>
<summary>X3. Chat GPT Prompt for generating Epics, User Stories, Acceptance Criteria and Tasks </summary>

```txt
Act as world class product owner, generate epics, user stories, acceptance criteria, and tasks for the following software feature:

the feature is create secure login for registered customers on our banking app.
```

#END</details>

<details>
<summary>A4. What is Business Analysis by IIBA? </summary>

## What is Business Analysis by IIBA?

### "The practice of enabling change in an enterprise by defining needs and recommending solutions that deliver value to the stakeholders"

- Understand the structure and dynamics of the company
- Technique of understanding business needs
- Solutions often revolve near to systems development, process improvement, strategic planning, and policy advancement
- Generating effective solutions
- Providing the required documentation 
- Assigning sufficient resources
- Achieving greater efficiency

#END</details>

<details>
<summary>A5. Importance of Business Analysis </summary>

# Importance of Business Analysis

The Benefits of Business Analysis:

- Analyze the business requirements
- Frame the proper planning
- Has particular pattern of documents
- Create adequate documentations
- Identify and develop various actions
- Improve the company standards

A Business Analyst involves himself (herself) in the implementation phase and also identifies various ways to reach the estimated goals. 
He/she plays an instrumental role throughout the project lifecycle and thereby increases the demand for business analysts in every organization.

#END</details>

<details>
<summary>1. What is Business Analysis? </summary>

# What is Business Analysis?



#END</details>

# COURSE

<details>
<summary>1. What is Business Analysis? </summary>

# What is Business Analysis?


#END</details>

<details>
<summary>2. What is Business Analysis? </summary>

# What is Business Analysis?


#END</details>
