# Business-Analysis

# RAW NOTES

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

# NOTES

<details>
<summary>A1. What is Business Analysis by IIBA? </summary>

## What is Business Analysis by IIBA?

### "The practice of enabling change in an enterprise by defining needs and recommending solutions that deliver value to the stakeholders"

- Understand the structure and dynamics of the company
- Technique of understanding business needs
- Solutions often revolve near to systems development, process improvement, strategic planning, and policy advancement
- Generating effective solutions
- Providing the required documentation 
- Assigning sufficient resources
- Achieving greater efficiency

### Business analysis is the practice of enabling change in an enterprise by defining needs and recommending solutions that deliver value to stakeholders.
### Business analysis enables an enterprise to articulate needs and the rationale for change, and to design and describe solutions that can deliver value.  - IIBA BABOK Guide v3
### Business analysis helps to bridge the gap between existing processes and growth. It is critical to learn to understand and refine a problem in order to determine and implement a solution.

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

# #END</details>

<details>
<summary>A2. Top Companies Using Business Analysis </summary>

# Top Companies Using Business Analysis

1. Accenture 
2. Cognizant
3. Deloitte
4. TATA CONSULTANCY SERVICES
5. KFORCE 
6. AMERICAN EXPRESS
7. Google 
8. DELL
9. amazon 
10. Flipkart

- System analysts mainly focus on creating and implementing specific systems with a more technical approach to the work.
- Data analysts help companies by analyzing data and using that data to perform proper actions to present value to the business stakeholders.
- Business analytics is usually dependent on data and reporting. It involves skills, technologies, past performance investigation, and information search.

# #END</details>

<details>
<summary>A3. How Is Business Analysis Performed? </summary>

# How Is Business Analysis Performed?

Business analysis is divided into multiple steps, with each phase having specific tasks to perform, principles to follow, and documents to produce.

1. Information Gathering
2. Discover Business Objectives
3. Define Scope
4. Business Analysis Plan
5. Define Detailed Requirements
6. Implementation
7. Access The Value Created by The Project

## Information Gathering 

This is the initial step where you lay the groundwork for your project.

Key Responsibilities:

- Clarifying your role as a business analyst 
- Identifying the primary stakeholders
- Understanding the history of your project
- Understanding the current systems and business processes

## Discover Business Objectives

In this particular step, the objectives and goals of the project are defined.

Key Responsibilities:

- Finding out the "why" behind the project.
- Finding out the expectations of your primary stakeholders.
- Making sure that the business objectives are clear and attainable.
- Solving the conflicting expectations so that everyone is on the same page.

## Define Scope

In this step, you need to define a clear, concise, and complete statement of scope.

Key Responsibilities:

- Verifying and confirming the business objectives to make sure that the organization is still investing in them
- Developing multiple strategies to figure out the suitable technology, shortlisting the options.
- Define the business process changes that are needed to implement the solution
- Drafting and reviewing scope statement

## Business Analysis Plan

Planning is necessary to make any project successful. Business analysts and the project owner can devise a proper plan to deliver the appropriate requirements. In the further stages of the project a business analysis plan will answer many questions for you and your project team. It will bring clarity to the business analysis process and help you define the detailed requirements for a project.

Key Responsibilities:

- Identifying the most appropriate types of business analysis deliverables
- Set up deadlines for completing these defined deliverables
- Check business analysis deliverables
- Complete the deliverables

## Define Detailed Requirements

After the planning process is done the requirements are defined. Make sure that requirements are clear, concise, concrete, complete and consistent.

Key Responsibilities:

- Gathering the information needed
- Analyzing the discovered requirements and creating a first draft that contains the one or more business analysis deliverables in detail 
- Outlining and validating each deliverable with appropriate technology
- Reviewing and validating deliverables

## Implementation

Implementing the solution is a crucial point. This step should proceed according to the way it was planned otherwise the project may get delayed. As an analyst you need to help the technical team in any way possible. 

Key Responsibilities:

- Analyzing the solution design to ensure it can fulfill all of the requirements stated by stakeholders
- Documenting the project so it will be useful for the technology design and implementation process
- Liaison between the business users and technical team. The Business analysts must answer every question and resolve the issues that may occur during the technical design implementation or testing phases 
- Assisting the team to accept the changes that might come up after all the steps are completed including the implementation part

## Access The Value Created by The Project

The last step is to check if the result obtained matches what you had expected. 

Key Responsibilities:

- Evaluating the progress against the business objectives
- Proposing follow-up plans
- Accessing the user engagement using various tools and techniques
- Delivering the results to the stakeholders

# #END</details>

<details>
<summary>A4. Roles & responsibilities of a Business Analyst</summary>

# Roles & responsibilities of a Business Analyst

## Roles of a Business Analyst

1. Multi-tasking
2. Reach the goal of the organization
3. Communicate with stakeholders
4. Determining a suitable way to improve the business processes
5. Implement new features
6. Identifying the ways to make the analysis easier

## Responsibilities of a Business Analyst

1. Understanding goals and problems
2. Meeting the organization's requirements
3. Analyzation
4. Communication
5. Implementation

## Knowledge areas of Business Analysis

- Business Analysis Planning and Monitoring 
- Elicitation and collaboration
- Enterprise Analysis
- Requirements Analysis 
- Solution Assessment and Validation 
- Requirements Management and Communication

# #END</details>

<details>
<summary>A5. Business Analysis techniques</summary>

# Business Analysis techniques

## MOST - Mission, Objectives, Strategies, and Tactics

- Analyzes the internal structures of what an organization aims to accomplish, and how to formulate the specific solutions.

## PESTLE Analysis - Political, Economic, Sociological, Technological, Legal and Environmental 

- Evaluates external factors that would impact business and determine how to address these factors if found.

## SWOT Analysis - Strengths, Weaknesses, Opportunities, Threats

- Involves structuring and categorizing processes into opportunities and threats.

## MOSCOW Analysis - Must or Should, Could or Would

- Allows for prioritizing requirements by presenting a framework in which each condition can be evaluated relative to others.

## CATWOE - Customers, Actors, Transformation Process, World View, Owner, and Environmental Constraints

- Helps business analysts understand different stakeholders' perspectives

# #END</details>

<details>
<summary>A6. Qualifications of a Business Analyst/BA Competencies</summary>

# Qualifications of a Business Analyst/BA Competencies

These include the following:

1. Analytical thinking - ﻿﻿Ability to Think critically and analytically.
2. Behavioral characteristics - Ethics, Trustworthiness, Time Management.
3. Business knowledge - Business Acumen, Industry Knowledge.
4. Communication - Strong interpersonal and communication skills
5. Interaction - ﻿﻿Observation skills, Attention to detail
6. Tools and technology - Office Suite Knowledge

###

1. Analytical thinking

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/1042dac2-744f-46dd-8181-4ed6f85b405b)

2. Behavioral characteristics

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/e4effd89-2cdc-468f-89ae-0940e38ba6da)

3. Business knowledge

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/74b6516d-dec9-417d-ae72-1516ab366643)

4. Communication

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/4a1bd86e-5d81-490c-abbb-acc125b0b754)

5. Interaction

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/9ea73a6a-62b4-4ffc-a71c-e71e81c1f8a9)

6. Tools and technology

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/f11946f3-39fd-4dc3-8319-542e2ca3e26b)

# #END</details>
        

# COURSE

<details>
<summary>1. Introduction to Business Analysis </summary>

# Introduction to Business Analysis

## Who are Business Analysts?

- Business Analysts were also called System Analysts.
- Business Analysts analyze Business Systems to enable change in an enterprise, by defining needs and recommending solutions that deliver value to stakeholders.
- Business Analysts gather requirements with respect to any changes to be made to Internal or External Business Systems.

## Types of Business Systems:

1. Internal System - These are systems used by employees or staff of the organisation. eg. Salesforce, POS Systems.
2. External System - These are systems used by the customers. eg. Self-Checkout Machines, A Company Website.

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/9237b3f4-da26-4443-a2bf-cc4d042ceb15)

## Types of Business System Changes:

1. New System - This is creating a stand-alone system or new product.
2. System Enhancement - This is adding more features or changes to an existing System.
3. System Re-engineering - This is completely upgrading the system to a new platform to replace the old system. Reverse Engineering can be used to capture requirements.

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/715673b1-34e6-4b1e-b672-63869a5f1d1f)
![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/03388173-8c21-45b8-97b1-086125806d0b)

## Successful Traits of a Business Analyst:

1. Interpersonal Skills - Ability to be a people person
2. Communication Skills
3. Listening Skills
4. Elicitation Skills - Ability to Ask Questions
5. Documentation Skills - Ability to Take Notes

## 2 Teams Business Analyst work with:

1. Business Team (Stakeholders)
2. IT Project Team

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/1c9fbad3-4977-460b-9d3e-6db71ade775c)

## Members of an IT Business Team

1. Project Manager
2. Business Analyst
3. System Architect
4. Developers or Programmers
5. Database Administrator (DBA)
6. Quality Assurance or Analyst (QA)

### Project Manager

- Manages the IT Team
- Makes sure the Project is completed in the given timeframe
- Defines budget based on Scope
- Provides status update of project

### Business Analyst

- Creates Requirements within Business Requirements document represented as - Functional Requirements Document(FRD), Use Cases, or User Stories

### Systems Analyst

- Creates System Design based on requirements

### Developers or Programmers

- Writes code based on requirements

### Database Administrator (DBA)

- Designs the Database and creates fields for inputs from the system
- Saves the Data in the Database

### Quality Assurance or Analyst (QA)

- Ensures that the changes made to the system meet the requirements
- Tests the system

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/71369790-4e5d-4046-bb4a-13465d816094)
![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/4f29d344-c52b-47c7-9d22-0c29e9628ce2)

# #END</details>

<details>
<summary>2. Documenting Business Requirements </summary>

# Documenting Business Requirements

## Who is a Business Owner

- A Business Owner is responsible for running the LOB of an Organisation.
- They identify the need of an IT Project
- They are the Project Sponsor
  
### LOB - Line of Business
### Project Sponsor - Financially responsible for the Project

![image](https://github.com/omeatai/src-Business-Analysis/assets/32337103/6a6725c9-9ad8-4a95-b82e-625c3aca2055)

<img width="929" alt="image" src="https://github.com/omeatai/src-Business-Analysis/assets/32337103/8acf0504-67d2-42ed-8210-a30c5f31d391">
<img width="929" alt="image" src="https://github.com/omeatai/src-Business-Analysis/assets/32337103/2b2959ed-84e7-41ba-b904-91c0b9c9db44">


# #END</details>



















