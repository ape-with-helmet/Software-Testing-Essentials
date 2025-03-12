# Software Testing Concepts 
## Table of Contents  
- [What is software? Types of softwares](#what-is-software-types-of-softwares)
- [What is software testing?](#what-is-software-testing)
- [Project Vs Product](#project-vs-product)
- [Why do we need testing?](#why-do-we-need-testing)
- [Error, bugs and failure](#error-bug--failure)
- [Why the software has bugs](#why-software-has-bugs)
- [Software Development Lifecycle](#software-development-lifecycle-sdlc)
    - [Waterfall Model](#waterfall-model)  
    - [Spiral Model](#spiral-model)  
    - [V-Model](#v-model)  
- [Review, Walkthrough & Inspection](#review-walkthrough--inspection)
- [QA & QC & QE](#qa--qc--qe)
- [Levels of Software testing](#levels-of-software-testing)
    - [Unit Testing](#unit-testing)
    - [Integration Testing](#integration-testing)
    - [System Testing](#system-testing)
    - [User Acceptance Testing](#user-acceptance-testing)
- [System Testing Types](#system-testing-types)
    - [GUI Testing](#graphical-user-interface-gui-testing)
    - [Usability Testing](#usability-testing)
    - [Functional Testing](#functional-testing)
    - [Non Functional Testing](#non-functional-testing)
- [Regression Testing](#regression-testing)
- [Re-Testing](#re-testing)
- [Smoke & Sanity Testing](#smoke--sanity-testing)
- [Exploratory Testing](#exploratory-testing)
- [Ad-hoc Testing](#ad-hoc-testing)
- [Monkey Testing](#monkeygorilla-testing)
- [Ad-hoc vs Exploratory vs Monkey Testing](#ad-hoc-vs-monkey-vs-exploratory-testing)
- [Positive & Negative Testing](#positive--negative-testing)
- [End to end Testing](#end-to-end-testing)
- [Globalization (I18N) & Localization Testing](#globalization-i18n-and-localization-testing)
- [Test Design Techniques](#test-design-techniques)
- [Software Testing Life Cycle](#software-testing-life-cycle-stlc)
- [Contents in Test Plan](#test-plan-contents)
- [Use case, Test Scenario & Test Case](#use-case-test-scenario--test-case)
- [What is a Test Case?](#what-is-a-test-case)
- [Requirements Traceability Matrix (RTM)](#requirement-traceability-matrix-rtm)
- [Environment & Execution](#environment--execution)
- [Defects/Bugs](#defectbugs)
- [Defect Classification](#defect-classification)
- [Defect Severity & Priority](#defect-severity--priority)
- [Defect Resolution](#defect-resolution)
- [Bug Life Cycle](#bug-life-cycle)
- [Test Cycle Closure](#test-cycle-closure)
- [Test Metrics](#test-metrics)
- [QA/Tester Responsibilities](#qatester-responsibilities)
## What is software? Types of softwares  

**Software** - A collection of computer programs that helps us to perform a task.  
**Types** - 
- **System software**: The base bones softwares which makes the computer what it is.  
    Ex: Device Drivers, Operating Systems, Servers, Utilities, etc.
- **Programming Software**: The softwares which allow us to write, build and execute the custom programs we want to make.  
    Ex: Compilers, Debuggers, Interpreters etc.
- **Application Software**: These are the softwares you and I build. The softwares which are used by most of the people, be it hosted on the cloud or be a native desktop app.  
    Ex: Web Applications, Mobile Applications, Desktop Applications.


## What is software testing?

- Software testing is a part of __software development process__.
- Software testing is an activity to detect and identify the defects in the software.
- The objective of testing is to release quality product to the client.

## What is Software quality?

* Bug-free
* Delivered on-time
* Within Budget
* Meets requirements and/or expectations.
* Maintainable

## Project Vs Product  

Although similar, there are small differences

**Project** - A Software developed for a specific/group of customer(s), whose requirements are given by the said customer and are usually taken up by Service based companies.

**Product** - A Software developed for a larger group of consumers (not customers), whose requirements are derived from the market rather than the customers themselves and are mostly taken up by the product based companies.

## Why do we need testing?

We conduct softwarer testing to ensure the product we build is in working condition and also is **devoid of bugs** and **meets the requirements**.  
Without software testing, we end up with software which is riddled with bugs and issues which will also lead to *customer dissatisfaction*.

## Error, Bug & Failure  

Although they sound similar, there are some technical differences.  
**Error** - An incorrect human action. Caused on the human end. (*Dev Phase*)  
**Bug** - A deviation from expected behaviour. Also called *Defect*. (*Testing Phase*)  
**Failure** - Deviation identified by end user is called failure. (*Deployment Phase*)  

## Why Software has bugs?

- Miscommunication or No communication.
- Software Complexity.
- Programming Errors.
- Changing Requirements. (**Major Cause**)
- Lack of skilled testers.

## Blackbox VS Whitebox testing  

Process of testing the product for the requirements rather than the code itself is called ***blackbox testing***. This is also called *functional testing*, where we just check the functionality of the product rather than the structure.  

Process of testing the product for the code itself and comparing how it should function and how it is functioning is called ***Whitebox testing***. Also called *Structural Testing*, where we check the structure of the program and not only 

## Software Development Lifecycle (SDLC)  

A *process* used by software industry to develop, test and deliver products to the customers.  
**P** - People  
**P** - Process  
**P** - Product  

This usually happens in different phases.
- Requirement analysis
- Design
- Development
- Testing
- Maintenance


### Waterfall Model

A traditional model, also called *Linear Model*. Not in use now.  
Documentation plays a key role in the entire process. Each and everything must be well documented.  

<img src='https://th.bing.com/th/id/OIP.nLzaXlAKLUGS16SCt_5V3AHaEK?rs=1&pid=ImgDetMain' alt='Waterfall model image' style="width:100%;">

Once the product owners gather all the requirements, they create **S**oftware **R**equirements **S**pecifications (**SRS**) document.  

System designers will break down the requirements into higher level and lower level models which will later be integrated. The Design document is created.  

Using the design document, the development is started, after which the testing is conducted.  

Once the testing phase is completed, the model is then deployed into the customer environment where it is used by the customer and the company will then only maintain the software to ensure it is in running condition all the time.

#### Advantages  
- Quality is good since there is detailed documentation for every phase which reduces miscommunications.
- Requirements are static which means that the bugs are less likely.
- Initial investment is less since the testers are hired at a later stage of development.
- Preferred for smaller projects where the requirements are frozen.

#### Disadvantages  
- Requirements are not changable.
- If there are errors in the requirements, it will continue into the later phases since it cannot be changed.
- Total investment is more since reworking defects will take more time and inturn cost lots of money.
- Testing will start only after the development is completed.

### Spiral Model

Also called iterative model.
<img src='https://artoftesting.com/wp-content/uploads/2020/01/spiral.jpg' alt='Spiral model image' style="width:100%;">

Goes through multiple levels of iterations, so that there is some level of free space to change requirements.

*Preferred by product based companies*

New features are built onto the previous version so that its an upgrade and not an entire rewamp. 

There needs to be dependancies on the requirements of the previous versions. Its hard to implement parts which have nothing to do with the previous versions.  

Every cycle, new software will be released to the customer. Each cycle follows waterfall model.

Software will be released in multiple versions which is why it is also called version control model.

#### Advantages

- Testing is done in every cycle, before going to the next cycle.
- Customer will get to use the softwarer for every module.
- Requirement changes are allowed after every cycle before going to the next cycle.

#### Disadvantages

- Requirement changes are **not** allowed during the cycle.
- Every cycle of spiral model looks like waterfall model.
- There is no testing in the requirements & design phase.


### V-Model

Also called VV-Model (*Verification & Validation Model*).  
Here, the software is divided into multiple smaller sections (*modules*) which are developed independantly and therefore can be tested individually as well.  
<img src='https://th.bing.com/th/id/R.a50335907cd6aadefb31b79e5bbca38f?rik=AM7vXqLZ3NYs6Q&riu=http%3a%2f%2fupload.wikimedia.org%2fwikipedia%2fcommons%2fb%2fb6%2fV-model-en.png&ehk=aFIMpAkcETOXbkH2i4QQ41jqClkq5zQxnzj8XPqkCM4%3d&risl=&pid=ImgRaw&r=0' alt='V model image' style="width:100%;">

The speciality of V-Model is that testing is conducted in every phase of software development. The processes are split into 2 parts, Verification and Validation.

<table>
    <tr>
     <th>Verification</th> 
     <th>Validation</th> 
    </tr>
    <tr>
        <td>(Business/Customer/User) Requirements Specification</td>
        <td>User Acceptance Testing (UAT)</td>
    </tr>
    <tr>
        <td>Software Requirements Specifications</td>
        <td>System Testing</td>
    </tr>
    <tr>
        <td>High/Low level Design Document</td>
        <td>Integration Testing</td>
    </tr>
    <tr>
        <td>Coding</td>
        <td>Unit Testing</td>
    </tr>
</table>

**Note:**  
*User Acceptance testing and System Testing come under Black box testing, and Integration testing and unit testing come under white box testing. All the documents must go through the following - Review, Walkthrough and Inspection.*

Testing the project related documents is called ***Static Testing***.  
The unit tests & integration tests are conducted by the developer herself. The System testing is done solely by the Testers while the UAT is done by the testers and the users themselves.  
The tests done on the actual software is called ***Dynamic Testing***  

#### Some differences between Verification and Validation.
<table>
    <tr>
     <th>Verification</th> 
     <th>Validation</th> 
    </tr>
    <tr>
        <td>Checks whether we are building the right product.</td>
        <td>Checks whether we are building the product right.</td>
    </tr>
    <tr>
        <td>Use static testing techniques.</td>
        <td>Use dynamic testing techniques.</td>
    </tr>
    <tr>
        <td>Takes place before validation.</td>
        <td>Takes place after verifications are completed.</td>
    </tr>
    <tr>
        <td>Focus on documentation.</td>
        <td>Focus on Software.</td>
    </tr>
    <tr>
        <td>
            Verification typically involves:
            <ul>
                <li>Reviews</li>
                <li>Walkthroughs</li>
                <li>Inspections</li>
            </ul>
        </td>
        <td>
            Validation typically involves:
            <ul>
                <li>Unit testing</li>
                <li>Integration testing</li>
                <li>System testing</li>
                <li>User Acceptance Testing</li>
            </ul>
        </td>
    </tr>
</table>  

#### Advantages 
- Testing is involved in each and every phase of the lifecycle

#### Disadvantages  
- Documentation is more.
- Initial investment is more.

***

## Review Walkthrough & Inspection
These are the 3 testing techniques used for static testing.

### Review
Reading through the entire document to check if the document is complete and checking if all the requirements are mentioned in the document.
Also to check if the content specified in the document is correct.

*Conducted on documents to ensure correctness and completeness.*

#### Types of review
- Requirement Reviews
- Design Reviews
- Code Reviews
- Test Plan Reviews
- Test Cases Reviews etc.

### Walkthrough 
It is in an informal review.  
Author reads the documents or code and discuss with peers.  
It's not pre-planned and can be done whenever required.  
Also walkthrough does not have minutes of the meet.  

### Inspection
It's the most formal review type.  
Requires invite to be sent to team, manager and almost everyone involved.  
At-least 3-8 people will sit in the meeting 
1. Reader (The author himself)
2. Writer (Write down all the questions and clarifications raised in the meeting)
3. Moderator (Organizer) plus concerned.  

Inspection will have a proper schedule which will be intimated via email to the concerned developer/tester.

## QA & QC & QE
### Quality Assurance vs Quality Control
<table>
    <tr>
        <th>QA</th>
        <th>QC</th>
    </tr>
    <tr>
        <td>Process related.</td>
        <td>Does the actual testing of the software.</td>
    </tr>
    <tr>
        <td>Focuses on building in quality.</td>
        <td>Focuses on testing for quality.</td>
    </tr>
    <tr>
        <td>Preventing defects.</td>
        <td>Finds defects.</td>
    </tr>
    <tr>
        <td>Process oriented.</td>
        <td>Product oriented.</td>
    </tr>
    <tr>
        <td>Required through the entire life cycle.</td>
        <td>Required for testing part of the SDLC.</td>
    </tr>
</table>

### Quality Engineering (QE)
The people who write automation test scripts are called quality engineer. They come under QC.

## Levels of Software Testing
- Unit Testing (Testing only a small part of the code)
- Integration Testing (Testing how the units interact with each other)
- System Testing (Testing how the entire system works as a whole)
- User Acceptance Testing (User should accept what is developed)

### Unit Testing 
A unit is a single component or a module of a software. Unit testing is done on a single program or a single module. Unit Testing is white box testing technique. Unit testing is conducted by the developers. When testing UI elements, we call it **component testing** rather than unit testing.  

Unit testing techniques:  
- Basis Path Testing
- Control Structure Testing
    - *Conditional Coverage*  
    - *Loops Coverage* 
- Mutation Testing

Some tools used for automation unit testing are JUnit, TestNV etc.

### Integration Testing
- Performed between 2 or more modules.
- Focuses on checking data communication between 2 or more modules.
- Part of white box testing.

There are 2 types of integration testing.
1. **Incremental Integration Testing** - Incrementally adding modules and testing the data flow between the modules. Two approaches within:
    - ***Top down approach***: Incrementally adding modules and testing the data flow between the modules but also ensure that the added module is a **child** of the previous module.
    - ***Bottom up approach***: Incrementally adding modules and testing the data flow between the modules but also ensure that the added module is a **parent** of the previous module.
    - ***Sandwich/Hybrid approach***: A combination of both top down and the bottom up approaches.
1. **Non Incremental Integration Testing** - Adding all modules in one single go and test the data flwo between modules.  
Drawbacks:
    - We might miss data flow between some of the modules.
    - If you find any defect we can't understand the root cause of defect. 

### System Testing
Tests all functionality of the application with respective client requirements.  
It is a black box testing technique.  
This testing is conducted by testing team.  
After completion of component and integration level testing, we start system testing.  
Before conducting system testing we should know the customer requirements.  

System Testing focuses on below aspects:
- User Interface Testing (GUI)
- Functional Testing
- Non-functional Testing (Involves performance testing and security testing etc.)
- Usability Testing

### User Acceptance Testing
After completion of the system testing, the UAT team conducts acceptance testing in 2 levels.
- Alpha Testing (User testing done in dev environment)
- Beta Testing (User testing done in customer environment)

After completion of these 2 tests, the software goes into production.

## System Testing Types
### Graphical User Interface (GUI) Testing
- Process of testing the user interface of an application. 
- A GUI includes all the elements such as the menu, checkboxes, buttons, colors, fonts, sizes, icons, content and images.

**GUI Testing Checklist:**
- Testing the size, position, width, height of elements.
- Testing of the error messages that are getting displayed.
- Testing the different sections of the screen.
- Testing of the font whether it is readable or not.
- Testing of the screen in different resolutions with the help of zooming in and zooming out.
- Testing the alignment of the texts and other elements like icons, buttons, etc. are in proper place or not.
- Testing the colors of the fonts.
- Testing whether the image has good clarity or not.
- Testing the alignment of the images.
- Testing the spelling.
- The user must not get frustrated while using the system interface.
- Testing whether the interface is attractive or not.
- Testing of the scrollbars according to the size of the page if any.
- Testing of the disables fields if any.
- Testing of the size of the images.
- Testing of the heading whether it is properly aligned or not.
- Testing of the color of the hyperlink.
- Testing UI elements like buttons, textbox, text area, checkbox, radio buttons, dropdowns, links etc.

### Usability Testing
- During this testing validates application provided context sensitive help or not to the user.
- Checks how easily the end users are able to understand and operate the application is called usability testing.
Works to check if the *User Manual*/Help menu of the website is helpful.

### Functional Testing
Functionality is nothing but behaviour of application.  
Functional testing talks about how your feature should work.  
- **Object Properties Testing**: Check the properties of objects present on the Application. Ex: disabled or not etc.
- **Database/Backend Testing**: Data Manipulation Language (DML) operations. Just checking if the Database operations work properly. Also can be classified as Grey box testing.

    - Table & Column level validations (Column type, column length, number of columns...)
    - Relation between tables (Normalization)
    - Functions
    - Procedures
    - Triggers
    - Indexes
    - Views etc.
- **Error Handling**: Tester verifies the error messages while performing incorrect actions on the application. Error messages should be readable and must be in simple/understandable language.
- **Calculations/Manipulations Testing**: Test the calculations within the application with valid and invalid data to verify if the application behaves properly.
- **Links Existence & Links Execution**: Are the links present and work as expected. 
    - **Internal Links**: Navigates somewhere in the same page.
    - **External Links**: Navigates to some other page.
    - **Broken Links**: Link exists but it does not redirect anywhere.
- **Cookies & Sessions**: Temporary files created by Browser while browsing the pages through internet are cookies. Cookies are created client side and sessions are created on the server side. Sessions are expired after some idle time.

### Non Functional Testing
Once the application functionality is stable then we do Non Functional Testing.  
Focus on performance, load it can take and security.

- **Performance Testing** (Speed of the website)
    - Load Testing: Increase the load on the application slowly and check the speed of the application.
    - Stress Testing: Suddenly increase/decrease the load on the application and check the speed of the application.
    - Volume Testing: Checking how much data can the application handle.
- **Security Testing**:
    - Authentication: Check if the users are valid.
    - Authorization: Allow valid users to access the application.
    - Access Control: Restrict the access levels based on the user permissions.
- **Recovery Testing**: Required time to recover data after loss of data.
- **Compatibility Testing**:
    - Forward Compatibility: Able to recieve future updates easily.
    - Backwards Compatibility: New updates should work on older devices despite the existence of newer devices. 
    - Hardware Compatibility (**Configuration Testing**): Checking if the software can install on multiple hardware configuration.
- **Installation Testing**: Testing the installation process to see if all the screens are easy to understand and the installation is simple. Check if the uninstallation deletes all related files.
- **Sanitation/Garbage Testing**: If any application provides extra features/functionality then we consider them as bug.

<table>
    <tr>
        <th>Functional Testing</th>
        <th>Non Functional Testing</th>
    </tr>
    <tr>
        <td>Validates functionality of Software</td>
        <td>Verify the performance, security, reliability of the software</td>
    </tr>
    <tr>
        <td>Functionality describes what software does</td>
        <td>Non-Functionality describes how software works</td>
    </tr>
    <tr>
        <td>Concentrates on user requirement</td>
        <td>Concentrates oon user expectation</td>
    </tr>
    <tr>
        <td>Functional testing takes place before non functional testing</td>
        <td>Non functional testing is performed after finishing Functional testing.</td>
    </tr>
</table>

## Regression Testing
Testing conducts on modified build to make sure there will not be impact on existing functionality because of changes like adding/deleting/modifying features.

### <span style="color:red;">Unit Regression Testing </span>
- Testing only the changes/modifications done by the developer
### <span style="color:red;">Regional Regression Testing </span>
- Testing the modified module along with thhe impacted modules
- Impact analysis meeting conducts to identify impacted modules with QA & Dev.
### <span style="color:red;">Full Regression</span>
- Testing the main feature & remaining part of the application
- Eg: Dev has done changes in many modules, instead of identifying impacted modules, we perform one round of full regression.

## Re-Testing
- Whenever the developer fixes a bug, tester will test the bug fix. This is called *Re-testing*.
- Tester clsoes the bug if it works otherwise re-opens and sends it to developer.
- To ensure that the defects which were found and posted in the earlier build were fixed and not in the current build.
- Example:
    - Build 1.0 was released. Test team found some defects (Defect id 1.0.1, 1.0.2) and posted.
    - Build 1.1 was released, now testing the defects 1.0.1 & 1.0.2 in this build is re-testing.

## Smoke & Sanity Testing
[Smoke](https://www.geeksforgeeks.org/smoke-testing-software-testing/) and [Sanity](https://www.geeksforgeeks.org/sanity-testing/) testing come into the picture after build release.
<table>
    <tr>
        <th>Smoke Testing</th>
        <th>Sanity Testing</th>
    </tr>
    <tr>
        <td>Smoke Test is done to make sure the build we recieved from the development team is testable/stable or not.</td>
        <td>Sanity Test is done during the release phase to check for the main functionalities of the application without going deeper.</td>
    </tr>
    <tr>
        <td>Smoke testing is performed by both Developers and Testers.</td>
        <td>Sanity testing is performed by Testers alone.</td>
    </tr>
    <tr>
        <td>During smoke testing, build may be either stable or unstable.</td>
        <td>During sanity testing, build is relatively stable.</td>
    </tr>
    <tr>
        <td>It is done on initial builds.</td>
        <td>It is done on stable builds.</td>
    </tr>
    <tr>
        <td>It is part of basic testing.</td>
        <td>It is part of regression testing.</td>
    </tr>
    <tr>
        <td>Usually it is done every time there is a new build release.</td>
        <td>It is planned when there is no enough time to do in-depth testing.</td>
    </tr>
</table>

## Exploratory Testing
- We have to explore the application, understand completely and test it.
- Understand the application, identify all possible scenarios, document it then use it for testing. 
- We do exploratory testing when the application ready but there is no requirement.
- Test engineer will do exploratory testing when there is no requirement.

### Drawbacks
- You might misunderstand any feature as a bug (or) any bug as a feature since you do not have requirement.
- Time consuming.
- If there is any bug in the application, you will never know about it.

## Ad-hoc Testing
- Testing application randomly without any test cases or any business requirement document.
- Ad-hoc testing is an informal testing type which an aim to break the system.
- Tester should have knowledge of the application even though he doesnt have requirements/test cases.
- This testing is usually an unplanned activity.

## Monkey/Gorilla Testing
- Testing application randomly without any test cases or any business requirement document.
- Ad-hoc testing is an informal testing type with an aim to break the system.
- Tester does not have knowledge of application
- Suitable for gaming application.

## Ad-hoc Vs Monkey Vs Exploratory Testing
<table>
    <tr>
        <th>Ad-hoc Testing</th>
        <th>Monkey Testing</th>
        <th>Exploratory Testing</th>
    </tr>
    <tr>
        <td>No Documentation</td>
        <td>No Documentation</td>
        <td>No Documentation</td>
    </tr>
    <tr>
        <td>No Plan</td>
        <td>No Plan</td>
        <td>No Plan</td>
    </tr>
    <tr>
        <td>Informal testing</td>
        <td>Informal testing</td>
        <td>Informal testing</td>
    </tr>
    <tr>
        <td>Tester should know Application functionality</td>
        <td>Tester doesn't know Application functionality</td>
        <td>Tester doesn't know Application functionality</td>
    </tr>
    <tr>
        <td>Random testing</td>
        <td>Random testing</td>
        <td>Random testing</td>
    </tr>
    <tr>
        <td>Intention is to break the application/find out corner defects</td>
        <td>Intention is to break the application/find out corner defects</td>
        <td>Intention is to learn or explore functionality of application</td>
    </tr>
    <tr>
        <td>Any Application</td>
        <td>Gaming Application</td>
        <td>Any Application which is new to tester</td>
    </tr>
</table>

## Positive & Negative Testing
### Positive Testing
- Testing the application with valid inputs is called Positive Testing.
- It checks whether an application behaves as expected with positive inputs.
- Eg: There is a text box in an application which can accept only numbers. Entering values up to 99999 will be acceptable by the system and any other values apart from this should not be acceptable.  
To do positive testing, set the valid input values from 0 to 99999 and check whether the system is accepting the values.

### Negative Testing
- testing the application with invalid inputs is called Negative Testing.
- It checks whether an application behaves as expected with the negative inputs.
- Eg: Negative testing can be performed by entering characters A to Z or from a to z. Either software system should not accept the values or else it should throw an error message for these invalid data inputs.

## End to End Testing
Testing the overall functionalities of the system including the data integration among all the modules is called end to end testing.

For a simple website, end to end testing would cover:
1. Login
1. **ADD** new customer
1. **EDIT** existing Customer
1. **DELETE** existing Customer
1. Logout

## Globalization (I18N) and Localization Testing
### Globalization Testing:
- Performed to ensure the system or software application can run in **any cultural or local environment**.
- Different aspects of the software applicationare tested to ensure that it supports every language and different attributes.
- It tests the different currency formats, mobile number formats and address formats are supported by the application.
- Eg: [www.facebook.com](https://www.facebook.com/) supports many of the languages and it can be accessed by people of different countries. Hence it is a global product.

### Localization Testing:
- Performed to check system or software application for a **specific geographical and cultural environment**.
- Localized product only supports the specific kind of language and is usable only in specific region.
- It tests the specific currency format, mobile number format and address format is working properly or not.
- Eg: baidu.com supports only the chinese language and can be accessed only by people of few countries. Hence it is a localized product.

## Test Design Techniques
Used to prepare data for testing. 
Use minimal data to cover most of the functionality.

    Important Note!

    Input Domain Testing: 
    The value will be verified in the text box/input fields. 
    ECP and BVA are used for this.

Types:
- **Equivalence Class Partitioning (ECP):**
    Partition data into various classes and we can select data according to clas then test. It reduces the number of test cases and saves time for testing.  
    - Value Checking
    - Classify/Divide/Partition the data into multiple classes.  

    Take a situation where there is an input which allows digits from 1-500.
        <table>
        <tr>
            <th>Normal Test Data</th>
            <th>Divide values into Equivalence Classes</th>
            <th>Test data using ECP</th>
        </tr>
        <tr>
            <td>1</td>
            <td>-100 - 0 => (<strong style="color:red;">Invalid</strong>)</td>
            <td>-50</td>
        </tr>
        <tr>
            <td>2</td>
            <td>1 - 100 => (<strong style="color:green;">Valid</strong>)</td>
            <td>30</td>
        </tr>
        <tr>
            <td>3</td>
            <td>101 - 200 => (<strong style="color:green;">Valid</strong>)</td>
            <td>160</td>
        </tr>
        <tr>
            <td>.</td>
            <td>201 - 300 => (<strong style="color:green;">Valid</strong>)</td>
            <td>250</td>
        </tr>
        <tr>
            <td>.</td>
            <td>301 - 400 => (<strong style="color:green;">Valid</strong>)</td>
            <td>320</td>
        </tr>
        <tr>
            <td>.</td>
            <td>401 - 500 => (<strong style="color:green;">Valid</strong>)</td>
            <td>450</td>
        </tr>
        <tr>
            <td>500</td>
            <td>501 - 600 => (<strong style="color:red;">Invalid</strong>)</td>
            <td>550</td>
        </tr>
    </table>

    Take another situation where the input allows only alphabets.
        <table>
        <tr>
            <th>Divide values into Equivalence Classes</th>
            <th>Test data using ECP</th>
        </tr>
        <tr>
            <td>A...Z => (<strong style="color:green;">Valid</strong>)</td>
            <td>XYZ</td>
        </tr>
        <tr>
            <td>a...z => (<strong style="color:green;">Valid</strong>)</td>
            <td>zyz</td>
        </tr>
        <tr>
            <td>Special Characters => (<strong style="color:red;">Invalid</strong>)</td>
            <td>@#$%</td>
        </tr>
        <tr>
            <td>Spaces => 250 (<strong style="color:red;">Invalid</strong>)</td>
            <td>Xy  z</td>
        </tr>
        <tr>
            <td>Numbers => 320 (<strong style="color:red;">Invalid</strong>)</td>
            <td>1234</td>
        </tr>
    </table>
- **Boundary Value Analysis (BVA):** We concentrate on the boundaries of the input.

    Take for example an input which allows digits 18-35.
    <table>
        <tr>
            <th>BVA Class</th>
            <th>Value</th>
            <th>Status</th>
        </tr>
        <tr>
            <td>Min - 1</td>
            <td>17</td>
            <td><strong style="color:red;">FAIL</strong></td>
        </tr>
        <tr>
            <td>Min</td>
            <td>18</td>
            <td><strong style="color:green;">PASS</strong></td>
        </tr>
        <tr>
            <td>Min + 1</td>
            <td>19</td>
            <td><strong style="color:green;">PASS</strong></td>
        </tr>
        <tr>
            <td>Nominal</td>
            <td>25</td>
            <td><strong style="color:green;">PASS</strong></td>
        </tr>
        <tr>
            <td>Max - 1</td>
            <td>34</td>
            <td><strong style="color:green;">PASS</strong></td>
        </tr>
        <tr>
            <td>Max</td>
            <td>35</td>
            <td><strong style="color:green;">PASS</strong></td>
        </tr>
        <tr>
            <td>Max + 1</td>
            <td>36</td>
            <td><strong style="color:red;">FAIL</strong></td>
        </tr>
    </table>
- **Decision Table based Testing:**
    - Also called Cause-Effect Table.
    - This technique will be used if we have more conditions and corresponding actions.
    - In decision table technique, we deal with combination of inputs.
    - To identify the test cases with decision table, we consider conditions and actions.

    Take an example of transferring money online to an account which is already added and approved.

    Here are the conditions to transfer the money:
    - Account already approved
    - OTP (One Time Password) matched
    - Sufficient money in the account

    And the actions performed are:
    - Transfer money
    - Show a message as insufficient amount
    - Block transaction in case of suspicious transaction

    <table>
        <tr>
            <td></td>
            <td></td>
            <td style="font-weight:700;">TC1</td>
            <td style="font-weight:700;">TC2</td>
            <td style="font-weight:700;">TC3</td>
            <td style="font-weight:700;">TC4</td>
            <td style="font-weight:700;">TC5</td>
        </tr>
        <tr>
            <td style="font-weight:700;">Condition 1</td>
            <td>Account already approved</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: red; font-weight:700;">FALSE</td>
        </tr>
        <tr>
            <td style="font-weight:700;">Condition 2</td>
            <td>OTP Matched</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: red; font-weight:700;">FALSE</td>
            <td style="color: red; font-weight:700;">FALSE</td>
            <td style="font-weight: 800;">X</td>
        </tr>
        <tr>
            <td style="font-weight:700;">Condition 3</td>
            <td>Sufficient money in the Account</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: red; font-weight:700;">FALSE</td>
            <td style="color: green; font-weight:700;">TRUE</td>
            <td style="color: red; font-weight:700;">FALSE</td>
            <td style="font-weight: 800;">X</td>
        </tr>
        <tr>
            <td style="font-weight:700;">Action 1</td>
            <td>Transfer Money</td>
            <td style="font-weight:700;">Execute</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td style="font-weight:700;">Action 2</td>
            <td>Show Message 'Insufficient Amount'</td>
            <td></td>
            <td style="font-weight:700;">Execute</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td style="font-weight:700;">Action 3</td>
            <td>Block the transaction incase of suspicious transaction</td>
            <td></td>
            <td></td>
            <td style="font-weight:700;">Execute</td>
            <td style="font-weight:700;">Execute</td>
            <td style="font-weight: 800;">X</td>
        </tr>
    </table>
- **State Transition:**
    - In state transition technique changes in input conditions change the state of the application
    - This testing technique allows the tester to test the behaviour of an SUT.
    - The tester can perform this action by entering various input conditions in a sequence.
    - In state transition technique, the testing team provides positive as well as negative input test values for evaluating the system behaviour.

    Take example of login page of an application which locks the user after 3 wrong attempts of password.
    <table>
        <tr style="background-color: green">
            <th>State</th>
            <th>Login</th>
            <th>Correct Password</th>
            <th>Incorrect Password</th>
        </tr>
        <tr>
            <td>S1</td>
            <td>First Attempt</td>
            <td style="color:green">S4</td>
            <td style="color:yellow">S2</td>
        </tr>
        <tr>
            <td>S2</td>
            <td>Second Attempt</td>
            <td style="color:green">S4</td>
            <td style="color:yellow">S3</td>
        </tr>
        <tr>
            <td>S3</td>
            <td>Third Attempt</td>
            <td style="color:green">S4</td>
            <td style="color:red">S5</td>
        </tr>
        <tr>
            <td>S4</td>
            <td style="color:green">Home Page</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>S5</td>
            <td style="color:red">Display a message as "Account locked, please consult admin"</td>
            <td></td>
            <td></td>
        </tr>
    </table>
- **Error Guessing:**
    - Error guessing is one of the testing techniques used to find bugs in a software application based on tester's prior experience.
    - In error guessing we dont follow any specific rules
    - It depends on tester's analytical skills and experience
    - Some of the examples are:
        - Submitting a form without entering values
        - Entering invalid values such as entering alphabets in the numeric field.

## Software Testing Life Cycle (STLC)
1. **Requirement Analysis**
1. **Test Planning**
1. **Test Design**
1. **Test Execution**
1. **Defect/bug reporting & Tracking**
1. **Test Closure**

<img src="https://miro.medium.com/v2/resize:fit:680/1*yB6uDks5ZoWb6IrJBIzPfw.jpeg" alt="Software Testing Life Cycle image" style="width:100%">

<table>
    <tr style="background-color: #FFD100; color: Black;">
        <th>Sl.No.</th>
        <th>PHASE</th>
        <th>Input</th>
        <th>Activities</th>
        <th>Responsibilities</th>
        <th>Outcome</th>
    </tr>
    <tr>
        <td>1</td>
        <td>Test Planning</td>
        <td>Project Plan</td>
        <td>Identify the Resources</td>
        <td>Test Lead/Team Lead (70%)</td>
        <td>Test Plan Document</td>
    </tr>
    <tr>
        <td></td>
        <td>What to test</td>
        <td>Functional Requirements</td>
        <td>Team Formation</td>
        <td>Test manager (30%)</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>How to test</td>
        <td></td>
        <td>Test Estimation</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td>When to test</td>
        <td></td>
        <td>Preparation of Test Plan</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td>Reviews on Test Plan</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td>Test plan sign off</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: black">
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>2</td>
        <td>Test Designing</td>
        <td>Project Plan</td>
        <td>Preparation of Test Scenarios</td>
        <td>Test Lead/Team Lead (30%)</td>
        <td>Test Cases Document</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Functional Requirements</td>
        <td>Preparation of Test Cases</td>
        <td>Test manager (70%)</td>
        <td>Traceability Matrix</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Test Plan</td>
        <td>Reviews on Test cases</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Design Docs</td>
        <td>Traceability Matrix</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Use Cases</td>
        <td>Test Cases Sign-off</td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: black">
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>3</td>
        <td>Test Execution</td>
        <td>Functional Requirements</td>
        <td>Executing Test Cases</td>
        <td>Test Lead/Team Lead (10%)</td>
        <td>Status/Test Reports</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Test Plan</td>
        <td>Preparation of Test Report/Test Log</td>
        <td>Test Engineers (90%)</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Test Cases</td>
        <td>Identifying Defects</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Build from Dev Team</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr style="background-color: black">
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>4</td>
        <td>Defect Reporting & Tracking</td>
        <td>Test Cases</td>
        <td>Preparation of Defect Report</td>
        <td>Test Lead/Team Lead (10%)</td>
        <td>Defect Report</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Test Reports/Test log</td>
        <td>Reporting Defects to developers</td>
        <td>Test Engineers (90%)</td>
        <td></td>
    </tr>
    <tr style="background-color: black">
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>5</td>
        <td>Test Closure/Sign-Off</td>
        <td>Test Reports</td>
        <td>Analysing Test Reports</td>
        <td>Test Lead/Team Lead (70%)</td>
        <td><strong>Test Summary Report</strong></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>Defect Reports</td>
        <td>Analysing Bug Reports</td>
        <td>Test Engineers (30%)</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td>Evaluating Exit Criteria</td>
        <td></td>
        <td></td>
    </tr>
</table>

## Test Plan Contents
A test plan is a document that describes the test scope, test strategy, objectives, schedule, deliverables and resources required to perform testing for a software product.  

<strong style="color:red;">Test plan template contents:</strong>
- Overview
- Scope
    - Inclusions
    - Test Environments
    - Exclusions
- Test Strategy
- Defect Reporting Procedure
- Roles/Responsibilities
- Test Schedule
- Test Deliverables
- Pricing
- Entry and Exit Criteria
- Suspension and Resumption Criteria
- Tools
- Risks and Mitigations
- Approvals

## Use case, Test Scenario & Test Case
### Use Case
- Use case describes the requirement.
- Use case contains 3 items:
    - **Actor**, which is the user, which can be a single person or a group of people, interacting with a process
    - **Action**, which is to reach the final outcome.
    - **Goal/Outcome**, which is the successful user outcome.

### Test Scenario
- A possible area to be tested (What to test)

### Test case
- Step by step actions to be performed to validate functionality of SUT (How to test)
- Test case contains test steps, expected results & actual result.

### Use Case V/s Test Case
- **Use case** - Describes functional requirement, prepared by Business Analyst (BA)
- **Test case** - Describes Test steps/Procedure, prepared by Test engineer.

### Test Scenario V/s Test Case  
Test Scenario is '**What to be tested**' and Test Case is '**How to be tested**'.  

Example:
- Test Scenario: Checking the functionality of Login Button
    - TC1: Click the button without entering username and password
    - TC2: Click the button only entering user name.
    - TC3: Click the button while entering wrong username and wrong password.

### Test Suite
Test Suite is a group of test cases which belong to the same category.
<img src="https://th.bing.com/th/id/R.7896b6360a562dc9155fb86d95abcef9?rik=n5ymeJNwQJ3knw&pid=ImgRaw&r=0" alt="Test Suite Image" style="width:100%;">

## What is a Test Case?  
A test case is set of actions executed to validate particular feature or functionality of your software application.

### Test case contents
- Test case ID
- Test case Title
- Description
- Pre-Condition
- Priority (P0, P1, P2, P3) - Order
- Requirement ID
- Steps/Actions 
- Expected result
- Actual result
- Test data

<table style="border: 1px solid;">
    <tr>
        <th style="border: 1px solid;">Tid</th>
        <th style="border: 1px solid;">Scenario</th>
        <th style="border: 1px solid;">Test Title</th>
        <th style="border: 1px solid;">Description</th>
        <th style="border: 1px solid;">Test Data</th>
        <th style="border: 1px solid;">Pre-Conditions</th>
        <th style="border: 1px solid;">Steps</th>
        <th style="border: 1px solid;">Expected Output</th>
        <th style="border: 1px solid;">Actual Output</th>
        <th style="border: 1px solid;">Status</th>
    </tr>
    <tr>
        <td style="border: 1px solid;">TC1</td>
        <td style="border: 1px solid;">Homepage</td>
        <td style="border: 1px solid;">Verify if property list is displayed when home page is loaded</td>
        <td style="border: 1px solid;">We verify if the homepage loads all the property data without applying any filters</td>
        <td style="border: 1px solid;">N/A</td>
        <td style="border: 1px solid;">
            <ol >
                <li>Open the browser</li>
                <li>Navigate to the website</li>
            </ol>
        </td>
        <td style="border: 1px solid;">
            <ol>
                <li>Login to the website</li>
                <li>Check if the page loads all the data</li>
            </ol>
        </td>
        <td style="border: 1px solid;">
            <ol>
                <li>Logs in and redirects to homepage.</li>  
                <li>Page loads all the property data.</li>
            </ol>
        </td>
        <td style="border: 1px solid;">
            <ol>
                <li>Logs in and redirects to homepage.</li>  
                <li>Page loads all the property data.</li>
            </ol>
        </td>
        <td style="border: 1px solid;">PASS</td>
    </tr>
</table>

## Requirement Traceability Matrix (RTM)
### What is RTM?
- RTM describes the mapping of requirements with the test cases.
- The main purpose of RTM is to see that all test cases are covered so that no functionality should miss while doing software testing.
- Requirements Traceability Matrix - Parameters include:
    - Requirement ID
    - Requirement Description
    - Test Case ID

### Sample RTM
<table style="border:1px solid;">
    <tr>
        <th style="border:1px solid;">Requirement No.</th>
        <th style="border:1px solid;">Requirement Description</th>
        <th style="border:1px solid;">Testcase ID</th>
        <th style="border:1px solid;">Status</th>
    </tr>
    <tr>
        <td style="border:1px solid;">123</td>
        <td style="border:1px solid;">Login to the application</td>
        <td style="border:1px solid;">TC01, TC02, TC03</td>
        <td style="border:1px solid;">
        TC01 - PASS<br>
        TC02 - PASS
        </td>
    </tr>
    <tr>
        <td style="border:1px solid;">345</td>
        <td style="border:1px solid;">Ticket Creation</td>
        <td style="border:1px solid;">
        TC04, TC05, TC06<br>
        TC07, TC08, TC09<br>
        TC010
        </td>
        <td style="border:1px solid;">
        TC04 - PASS<br>
        TC05 - PASS<br>
        TC06 - PASS<br>
        TC07 - FAIL<br>
        TC08 - NO RUN
        </td>
    </tr>
    <tr>
        <td style="border:1px solid;">456</td>
        <td style="border:1px solid;">Search Ticket</td>
        <td style="border:1px solid;">
        TC011, TC012,<br> 
        TC013, TC014
        </td>
        <td style="border:1px solid;">
        TC011 - PASS<br>
        TC012 - FAIL<br>
        TC013 - PASS<br>
        TC014 - NO RUN
        </td>
    </tr>
</table>


## Environment & Execution
### Test Environment 
- Test environment is a platform specially built for test case execution on the software product.
- It is created by integrating the required software and hardware along with proper network configurations.
- Test environment simulates production/real time environment.
- Another name for test environment is **Test Bed**.

### Test Execution
- During this phase test team will carry out the testing based on the test plans and the test cases prepared.
- **Entry Criteria:** Test cases, Test data & Test plan
- **Activities**:
    - Test cases are executed based on the test planning.
    - Status of test cases are marked, like Passed, Failed, Blocked, Run and others.
    - Documentation of test results and log defects for failed cases is done.
    - All the blocked and failed test cases are assigned bug ids.
    - Retesting once the defects are fixed. 
    - Defects are tracked till closure.
- **Deliverables**: Provides defect and test case execution report with completed results. 

### Guidelines for Test Execution
- The build being deployed to the QA environment is the most important part of the test execution cycle.
- Test execution is done in QA environment.
- Test execution happens in multiple cycles.
- Test execution phase consists Executing the test cases + test scripts (if automation)

## Defect/Bugs
- Any mismatched functionality found in an application is called Defect/Bug/Issue.
- During test execution, test engineers are reporting mismatches as defects to developers through templates or using tools.
- Defect reporting tools:
    - Clear Quest
    - DevTrack
    - Jira
    - Quality Center
    - Bug Jilla etc.
### Bug reporting contents
- Defect_ID - Unique identification number for the defect
- Defect Description - Detailed description of the defect including information about the module in which defect was found.
- Version - Version of the application in which defect was found.
- Steps - Detailed steps along with screenshots with which the developer can reproduce the defects.
- Date Raised - Date when the defect was raised.
- Reference - Where you provide reference to documents like requirements, design, architecture or maybe even screenshots of the error to help understand the defect.
- Detected by - Name/ID of the tester who raised the defect.
- Status - Status of the defect.
- Fixed by - Name/ID of the developer who fixed it.
- Date closed - Date when the defect is closed.
- Severity - Describes the impact of the defect on the application.
- Priority - Shows the urgency of the defect. Can be High/Medium/Low based on the impact urgency at which the defect should be fixed.

## Defect Classification
<table style="border:1px solid; width:100%">
    <tr>
        <th>Defects Categorization</th>
        <th></th>
    </tr>
    <tr>
        <th style="border:1px solid;">Severity</th>
        <th style="border:1px solid;">Priority</th>
    </tr>
    <tr>
        <td style="border:1px solid; background-color:red;">Blocker</td>
        <td style="border:1px solid; background-color:red;">P1</td>
    </tr>
    <tr>
        <td style="border:1px solid; background-color:orange;">Critical</td>
        <td style="border:1px solid; background-color:orange;">P2</td>
    </tr>
    <tr>
        <td style="border:1px solid; background-color:grey">Major</td>
        <td style="border:1px solid; background-color:#45b6fe">P3</td>
    </tr>
    <tr>
        <td style="border:1px solid;">Minor</td>
        <td style="border:1px solid;"></td>
    </tr>
</table>

## Defect Severity & Priority
### Defect Severity
Severity describes the seriousness of defect and how much impact on Business workflow.  
Defect severity can be categorized into 4 classes:
- **Blocker (Show stopper)**: This defect indicates nothing can proceed further.
    - Eg: Application crashed, Login not working etc.
- **Critical**: The main.basic functionality is not working. Customer business workflow is broken. They cannot proceed further.
    - Eg1: Fund transfer is not working in net banking
    - Eg2: Ordering product in ecommerce application is not working
- **Major**: It causes some undesirable behaviour, but the feature/application is still functional.
    - Eg1: After sending email there is no confirm message
    - Eg2: After booking cab there is no confirmation
- **Minor**: It won't cause any major break-down of the system
    - Ex: Look and feel issues, spelling, alignments.

### Defect Priority
Priority describes the importance of defect.  
Defect Priority states the order in which a defect should be fixed.  
Defect priority can be categorized into 3 classes:
- **P0 (HIGH):** The defect must be resolved immediately as it affects the system severely and cannot be used until it is fixed.
- **P1 (MEDIUM):** It can wait until a new version/build is created.
- **P2 (LOW):** Developer can fix it in later releases. 

### High severity, priority & Low severity, priority defects
<img src="https://th.bing.com/th/id/R.cd461852862fc479b37a2a45f021a1a1?rik=XyK14IwWGW5%2bAg&riu=http%3a%2f%2fwww.softwaretestingclass.com%2fwp-content%2fuploads%2f2012%2f08%2fdifference-between-Priority-and-Severity1.jpg&ehk=3TnifyhPqdd0epvDJqH3upRxoYtyO5EgPXRAtCE%2fjXk%3d&risl=&pid=ImgRaw&r=0&sres=1&sresct=1" alt="priority severity matrix" style="width:100%;">

**Examples**  
- **Low Priority - Low severity:** A spelling mistake in a page not frequently navigated by users.
- **Low Priority - High severity:** Application crashing in some very corner case.
- **High Priority - Low severity:** Slight change in logo color or spelling mistake in company name.
- **High Priority - High severity:** Issue with login functionality. (user unable to login to the application)
- **High Priority - Low severity:** Web page not found when user clicks on a link. (User does not visit that page generally)
- **Low Priority - Low severity:** Any cosmetic or spelling issues which is within a paragraph or in a page.

## Defect Resolution
After recieving the defect report from the testing team, development team conduct a review meeting to fix defects. Then they send a Resolution Type to the testing team for further communication.  

Resolution types:
- Accept
- Reject
- Duplicate
- Enhancement
- Need more information
- Not Reproducible
- Fixed
- As Designed

## Bug Life Cycle
<img style="width:100%;" alt="Bug Life Cycle Image" src="https://www.educba.com/academy/wp-content/uploads/2020/02/bug-life-cycle.jpg">

When the tester finds the bug, it is in "NEW" state.  
The dev project manager analyses the bug and if they deem it invalid, it is put in "REJECTED" state. Reject reasons could be Enhancement, Need more Info, Not reproducible, As Designed etc. Otherwise a check is done to see if the bug is already documented.  
If yes, then it is put in "DUPLICATE" state.  
If it is a new bug, then it is either "ASSIGNED" or "DEFERRED" based on priority and previous work load.  
When the developer starts fixing the bug, it is put in "OPEN" state.  
It is then changed to "FIXED" when the dev finishes the fix.  
The tester retests the bug and if they find the bug again, the bug is put back in "OPEN" otherwise it is put in "CLOSE" and regression testing is conducted.  
If the regression fails, the bug is "OPEN" again.  

## Test Cycle Closure
### Activities
- Evaluate cycle completion criteria based on Time, Test coverage, Cost, Software, Critical Business Objectives, Quality.
- Prepare test metrics based on the above parameters.
- Document the learning out of the project
- Prepare Test summary report
- Qualitative and Quantitative reporting of quality of the work product to the customer.
- Test result analysis to find out the defect distribution by type and severity.

### Deliverables
- Test Closure report
- Test Metrics


## Test Metrics
<table>
    <tr>
        <th>SNO</th>
        <th>Required Data</th>
    </tr>
    <tr>
        <td>1</td>
        <td>No of requirements</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Avg. no. of Test Cases written per Requirement</td>
    </tr>
    <tr>
        <td>3</td>
        <td>Total no. of Test Cases written for all Requirements</td>
    </tr>
    <tr>
        <td>4</td>
        <td>Total no. of Test Cases Executed</td>
    </tr>
    <tr>
        <td>5</td>
        <td>No. of Test cases passed</td>
    </tr>
    <tr>
        <td>6</td>
        <td>No. of Test cases failed</td>
    </tr>
    <tr>
        <td>7</td>
        <td>No. of Test cases blocked</td>
    </tr>
    <tr>
        <td>8</td>
        <td>No. of Test cases Un Executed</td>
    </tr>
    <tr>
        <td>9</td>
        <td>Total no. of defects identified</td>
    </tr>
    <tr>
        <td>10</td>
        <td>Critical defects count</td>
    </tr>
    <tr>
        <td>11</td>
        <td>Higher defects count</td>
    </tr>
    <tr>
        <td>12</td>
        <td>Medium defects count</td>
    </tr>
    <tr>
        <td>13</td>
        <td>Low defects count</td>
    </tr>
    <tr>
        <td>14</td>
        <td>Customer Defects</td>
    </tr>
    <tr>
        <td>15</td>
        <td>No. of defects found in UAT</td>
    </tr>
</table>

Here are some of the most important metrics used to evaluate test effectivity.
- **% of Test cases Executed:**  *(No of Test cases Executed / Total No of test cases written) * 100*
- **% of Test cases NOT Executed:**  *(No of Test cases NOT Executed / Total No of test cases written) * 100*
- **% of Test cases passed:**  *(No of Test cases passed / Total No of test cases executed) * 100*
- **% of Test cases failed:**  *(No of Test cases failed / Total No of test cases executed) * 100*
- **% of Test cases blocked:**  *(No of Test cases blocked / Total No of test cases executed) * 100*
- **Defect Density**: No of defects identified per requirement/s  
    *No. of defects found / Size(No. of requirements)*
- **Defect Removal Efficiency (DRE):**  
    *(A / A+B ) * 100*  
    *(Fixed Defects / (Fixed Defects + Missed Defects)) * 100*  
    - A - Defects identified during testing / Fixed Defects
    - B - Defects identified by customer / Missed Defects
- **Defect Leakage:** *(No. of defects found in UAT / No. of defects found in Testing) * 100*
- **Defect Rejection Ratio:** *(No. of defects rejected / Total no. of defects raised) * 100*
- **Defect Age:** *Fixed Date - Reported Date*
- **Customer Satisfaction:** *No. of complaints per period of time*

## QA/Tester Responsibilities
### QA/Testing Activities
- Understanding the requirements and functional specifications of the application.
- Identifying required Test Scenarios.
- Designing Test Cases to validate application
- Setting up Test environment (Test Bed)
- Execute Test Cases to validate application
- Log Test results (How many test cases pass/fail)
- Defect reporting and tracking
- Retest fixed defects of previous build
- Perform various types of testing on application
- Reports to Test Lead about the status of assigned tasks
- Participate in regular team meetings
- Creating automation scripts
- Provides recommendation on whether or not the application/system is ready for production

### 7 Principles of Software Testing
1. Start software testing at early stages. Means from the beginning when you get the requirements.
1. Test the software in order to find the defects.
1. Highly impossible to give the bug free software to the customer.
1. Should not do exhaustive testing. Means we should not use same type of data for testing every time.
1. Testing is context based. Which means what types of testing should be conducted must be based on type of application.
1. We should follow the concept of [Pesticide Paradox](https://katalon.com/resources-center/blog/pesticide-paradox-in-software-testing). If we are executing same test cases for longer runs, we wont find any defects. We have to update test cases in every cycle/release in order to find more defects
1. We should follow [defect clustering](https://www.geeksforgeeks.org/overview-of-defect-clustering/). Which means that some of the modules contains most of the defects. By experience, we can identify such risky modules. 80% of the problems are found in 20% of the modules
