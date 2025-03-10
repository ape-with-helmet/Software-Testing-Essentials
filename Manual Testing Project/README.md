# Manual Testing Project

## Table of Contents

- [Project Introduction](#project-introduction)
- [Understanding & Explore the Functionality](#understanding--explore-the-functionality)
- [Estimation](#estimation)
- [Test Plan](#test-plan)
- [Writing Test Scenarios](#writing-test-scenarios)
- [Writing Test cases, Reviews & RTM](#writing-test-cases-reviews--rtm)
- [Environment Setup & Build deployment](#environment-setup--build-deployment)
- [Test Execution](#test-execution)

## Project Introduction

We will be testing an **e-commerce** product/Application.  
You as a customer should be able to do the following:

- Login
- Search for products/items
- Add them to cart
- Do payment
- Product should be delivered
- Return product etc.

For any **e-commerce** project, there will be 2 parts:

1. **Front-end:** The part of the project which is visible to the public and is the interface through which the user interacts. Since this can be accessed across organizations, it is called an _Internet Application_.
2. **Back-end:** The part of the project which is available only to the admin in their environment. Customer cannot access this part of this project. Since this can be accessed only within the organization, it is called an _Intranet Application_.

As part of our project, we will be working with only the frontend.  
The product we will be testing for our project is [Open Cart](https://demo.opencart.com/).

## Understanding & Explore the Functionality

Since usually we never get the application in hand before creating the test plan, we must rely on documents like **[SRS documents](https://www.geeksforgeeks.org/software-requirement-specification-srs-format/)** to create our test plan.  
Check out the [Youtube Link](https://youtu.be/vv2PskqvGRA?list=PLUDwpEzHYYLseflPNg0bUKfLmAbO2JnE9&t=1450) to actually view the frs document. The document will contain all the functional requirements, may contain some mock up screens to show how the product should look like. Highlight the requirements on this document as we will be using this to write our test cases. We do estimation also at this point in time.

## Estimation

We make a estimation of the time and effort required to complete the project/test plan.  
There are multiple techniques to estimate the process of testing. **[Read more](https://www.geeksforgeeks.org/software-testing-estimation-techniques/)**

## Test plan

**[Test plan document](https://www.geeksforgeeks.org/test-plan-software-testing/)** contains all the details regarding the testing for the entire project like who will be testing what and when. This [link](https://youtu.be/vv2PskqvGRA?list=PLUDwpEzHYYLseflPNg0bUKfLmAbO2JnE9&t=2385) will take you to when the test plan document is shown.

The Test plan will contain the following things usually:

- Overview
- Scope
  - Inclusions
  - Test environments
  - Exclusions
- Test Strategy
- Defect Reporting Procedure
- Roles/Responsibilities
- Test Schedule
- Test Deliverables
- Pricing
- Entry and Exit Criteria
- Suspensions and Resumption Criteria
- Tools
- Risks and Mitigations
- Approvals

## Writing Test Scenarios

Sample Test scenarios

<table>
    <tr>
        <th style="background-color: green; border: 1px solid;">Project Name</th>
        <td style="border: 1px solid;">OpenCart (Frontend)</td>
    </tr>
    <tr>
        <th style="background-color: green; border: 1px solid;">Client</th>
        <td style="border: 1px solid;">OpenCart</td>
    </tr>
    <tr>
        <th style="background-color: green; border: 1px solid;">Reference Document</th>
        <td style="border: 1px solid;">FRS</td>
    </tr>
    <tr>
        <th style="background-color: green; border: 1px solid;">Created By</th>
        <td style="border: 1px solid;">Author_Name</td>
    </tr>
    <tr>
        <th style="background-color: green; border: 1px solid;">Created Date</th>
        <td style="border: 1px solid;">Authored_Date</td>
    </tr>
    <tr>
        <th style="background-color: green; border: 1px solid;">Approval Date</th>
        <td style="border: 1px solid;"></td>
    </tr>
</table>
<table>
    <tr>
        <th style="background-color: green; border: 1px solid;">Test Scenario ID</th>
        <th style="background-color: green; border: 1px solid;">Reference</th>
        <th style="background-color: green; border: 1px solid;">Test Scenario Description</th>
        <th style="background-color: green; border: 1px solid;">Priority</th>
        <th style="background-color: green; border: 1px solid;">Number of Test Cases</th>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_001</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Register Account functionality</td>
        <td style="border: 1px solid;">P0</td>
        <td style="border: 1px solid;">27</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_002</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Login functionality</td>
        <td style="border: 1px solid;">P0</td>
        <td style="border: 1px solid;">23</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_003</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Logout functionality</td>
        <td style="border: 1px solid;">P0</td>
        <td style="border: 1px solid;">11</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_004</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Forgot Password functionality</td>
        <td style="border: 1px solid;">P2</td>
        <td style="border: 1px solid;">25</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_005</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Search functionality</td>
        <td style="border: 1px solid;">P1</td>
        <td style="border: 1px solid;">22</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_006</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the working of Product Compare functionality</td>
        <td style="border: 1px solid;">P4</td>
        <td style="border: 1px solid;">24</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">.<br>.<br>.</td>
        <td style="border: 1px solid;">.<br>.<br>.</td>
        <td style="border: 1px solid;">.<br>.<br>.</td>
        <td style="border: 1px solid;">.<br>.<br>.</td>
        <td style="border: 1px solid;">.<br>.<br>.</td>
    </tr>
    <tr>
        <td style="border: 1px solid;">TS_032</td>
        <td style="border: 1px solid;">FRS</td>
        <td style="border: 1px solid;">Validate the complete Application functionality for different currencies</td>
        <td style="border: 1px solid;">P2</td>
        <td style="border: 1px solid;">3</td>
    </tr>
</table>

## Writing Test cases, Reviews & RTM

[Video link at time stamp](https://youtu.be/igyIAi0GND8?list=PLUDwpEzHYYLseflPNg0bUKfLmAbO2JnE9&t=191)

The document needs to contain a version history to show the changes made previously.  
Template will look like this

<table>
    <tr>
        <th style="background-color: darkgreen; border: 1px solid;">Project Name</th>
        <td style="border: 1px solid;">OpenCart</td>
    </tr>
    <tr>
        <th style="background-color: darkgreen; border: 1px solid;">Prepared By</th>
        <td style="border: 1px solid;">Author_Name</td>
    </tr>
    <tr>
        <th style="background-color: darkgreen; border-top: 1px solid; border-left: 1px solid; border-right: 1px solid; border-bottom: None;">Version No.</th>
        <td style="border: 1px solid;">Version 1.0</td>
        <td style="border: 1px solid;"></td>
    </tr>
    <tr>
        <th style="background-color: darkgreen; border-top: None; border-left: 1px solid; border-right: 1px solid; border-bottom: None;"></th>
        <td style="border: 1px solid;">Version 2.0</td>
        <td style="border: 1px solid;">Updated with Client Feedback</td>
    </tr>
    <tr>
        <th style="background-color: darkgreen; border-top: None; border-left: 1px solid; border-right: 1px solid; border-bottom: 1px solid;"></th>
        <td style="border: 1px solid;">Version 3.0</td>
        <td style="border: 1px solid;">Added Test Cases for new functionalities</td>
    </tr>
</table>

You can organise the test cases by separating them into different sheets according to the test scenarios.

### Example Test Case
<table>
    <tr>
        <th style="background-color: darkgreen; border:1px solid;">Test Case ID</th>
        <th style="background-color: darkgreen; border:1px solid;">Test Scenario</th>
        <th style="background-color: darkgreen; border:1px solid;">Test Case Title</th>
        <th style="background-color: darkgreen; border:1px solid;">Pre-requisites</th>
        <th style="background-color: darkgreen; border:1px solid;">Test Steps</th>
        <th style="background-color: darkgreen; border:1px solid;">Test Data</th>
        <th style="background-color: darkgreen; border:1px solid;">Expected Output</th>
        <th style="background-color: darkgreen; border:1px solid;">Actual Output</th>
        <th style="background-color: darkgreen; border:1px solid;">Priority</th>
        <th style="background-color: darkgreen; border:1px solid;">Status</th>
    </tr>
    <tr>
        <td style="border: 1px solid;">TC_RF_001</td>
        <td style="border: 1px solid;">(TS_001)<br>Register<br>Functionality</td>
        <td style="border: 1px solid;">Validate Registering an account by providing only the Mandatory fields</td>
        <td style="border: 1px solid;">1. Open the Application <a href="https://demo.opencart.com">website link</a> in any browser</td>
        <td style="border: 1px solid;">
            1. Click on 'My Account' drop menu<br>
            2. Click on 'Register' option<br>
            3. Enter new account details into the mandatory fields (First Name, Last Name, email, telephone, password, password confirm and privacy policy fields)<br>
            4. Click on 'Continue' button <strong>(ER-1)</strong><br>
            5. Click on 'Continue' button that is displayed in the 'Account Success' page <strong>(ER-2)</strong>
        </td>
        <td style="border: 1px solid;">Not Applicable</td>
        <td style="border: 1px solid;">
            1. User should be logged in, taken to 'Account Success' page and proper details should be displayed on the page<br>
            2. User should be taken to 'Account' page and a confirm email should be sent to the registered email address.
        </td>
        <td style="border: 1px solid;"></td>
        <td style="border: 1px solid;"></td>
        <td style="border: 1px solid;"></td>
    </tr>
</table>

Execute the test cases one by one and mark them as passed or failed.  
Do the test cases by yourself by using the youtube link as reference.  

    The entire RTM must be done in a single sheet.
    RTM will specify if a particular requirement is covered or not.
There will be multiple reviews for the test cases.

## Environment Setup & Build deployment
**[Timestamp](https://youtu.be/DtMOd8RDy20?list=PLUDwpEzHYYLseflPNg0bUKfLmAbO2JnE9&t=2581)**  
To test the database part and the backend admin part, we need to download the project and set it up in our environment and build it. The *test environments* are mentioned in the **Test Plan** and the *technologies used* are mentioned in the **FRS** document

To deploy this particular application, we need to have **MySQL Database** and **Apache server**. We could alternatively use **XAMPP** to run the database and control the database server.

It is **Highly Recommended** to do this part along with the video linked at the start of this chapter.

### OpenCart Build Deployment
#### Relevant Links
1. [OpenCart Download Link](https://www.opencart.com/index.php?route=cms/download)
2. XAMPP for apache, mysql and php installation (Download the latest stable version) [Download Link](https://www.apachefriends.org/download.html)

#### Installing and setting up XAMPP
1. Install the latest version which is available for your operating system.
1. Run the installation file you just downloaded.
1. Click next while keeping default settings and once it finishes installing, click on finish and start the XAMPP control panel.
1. Now click on start on Apache and MySQL. Ensure you dont close the control panel when server is running.

#### Installing the OpenCart app
1. Open the link and click on the Download and host your own button which should get you a **.zip** file.
1. Extract the **.zip** file into <code>C:\xampp\htdocs</code> which once extracted should have a path that looks something like <code>C:\xampp\htdocs\opencart-3.0.3.6</code>
1. Rename the folder into **opencart** which should make the path look like <code>C:\xampp\htdocs\opencart</code>
1. Go to <code>C:\xampp\htdocs\opencart\upload</code> and rename **config-dist.php** -> **config.php**.
1. Similarly, go to <code>C:\xampp\htdocs\opencart\upload\admin</code> and rename **config-dist.php** -> **config.php**.
1. We now connect to the [Database](http://localhost/phpmyadmin/) and create a database **openshop** while using Collation.
1. Now open the [website](http://localhost/opencart) and click on **upload**.
1. Click on continue and check if all the requirements are met and click continue again.
1. Now we provide the **Database Connection details**
    - **Hostname** - <code>localhost</code>
    - **Username** - <code>root</code>
    - **Password** - *Leave Blank*
    - **Database** - <code>openshop</code>
    - **Port** - <code>3306</code>
    - **Admin Details** - Use any name, email and password but do remember what you have entered.
1. Click on continue.
1. Go to <code>C:\xampp\htdocs\opencart\upload</code> and delete the **install** folder.
1. Now we can go to the [Shop page](http://localhost/opencart/upload) or the [Admin page](http://localhost/opencart/upload/admin).

**Congratulation!** OpenCart is now up and running in your local system.  
To view the tables, go back to [phpmyadmin](http://localhost/phpmyadmin) and open the **openshop** database, which should have all the necessary tables imported.

The installation itself can be a form of smoke testing which if failed, the developer must deliver another build.

## Test Execution
<iframe width="1536" height="960" src="https://www.youtube.com/embed/SB0g8wkPz9o?list=PLUDwpEzHYYLseflPNg0bUKfLmAbO2JnE9" title="Manual Software Testing LIVE Project Part-4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="width:100%"></iframe>
It is important to stick to the test plan during execution.