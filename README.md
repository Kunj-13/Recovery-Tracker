# Recovery Tracker
 
## Project Objectives

The objective of our project is to develop a software application that aids in understanding, managing, and combating drug abuse and addiction. By leveraging data structures and algorithms, the application provides a user-friendly interface for individuals to record and track personal recovery milestones, monitor health metrics, and maintain a journal of their rehabilitation journey. This tool aims to support users in their recovery process by offering a structured way to visualize progress and setbacks, thus facilitating a better understanding of their personal addiction patterns.

**Key Objectives:**

- Personal Recovery Monitoring: Implement features that allow users to record and monitor their daily recovery activities. This includes tracking sobriety milestones, journaling daily experiences, and noting any relapses or challenges. The main-8.py script in our application facilitates this by enabling users to add and view personal milestones and health metrics, offering a clear picture of their recovery journey over time.
- **Health Metrics Visualization:** Provide tools for users to input and visualize various health metrics, such as mood, cravings, and overall wellbeing. This functionality, handled by user_module.py, helps users and their healthcare providers observe patterns and make informed decisions based on solid data.
- **Secure and Private User Management:** Through the **admin_module.py**, our application ensures secure user registration and authentication processes, maintaining the confidentiality of personal and sensitive data. This is crucial for building trust and ensuring user comfort in sharing personal information.
- **Accessibility and Ease of Use**: Design the application to be user-friendly, allowing users of all technological skill levels to easily navigate and utilize the various features without feeling overwhelmed. This is achieved by straightforward menu options and clear instructions within the application, as managed by the main control script main.py.
-**Support and Resources**: Apart from tracking and data visualization, provide users with access to educational resources and support options. This helps in not only managing their addiction but also understanding it better, fostering a comprehensive approach to recovery.

## Significance Of The Project

Our project, centered around developing a comprehensive software application for managing drug abuse and addiction recovery, stands out for its meaningful contribution to public health and personal well-being. Unlike traditional treatment tracking tools, our application introduces an innovative blend of personal journaling, milestone tracking, and health metrics visualization. This triad of features not only assists individuals in monitoring their recovery but also provides healthcare providers with actionable insights into their patients' progress.

The novelty of our application lies in its user-centric design, which emphasizes privacy, user-friendliness, and comprehensive support. By integrating these elements, we offer a personalized recovery experience that is adaptable to the unique needs of each user. Our application goes beyond mere data tracking; it empowers users to gain a deeper understanding of their behavioral patterns and the effectiveness of their treatment plans. This insight is crucial for making informed adjustments that enhance recovery outcomes. Also, our project leverages advanced data structures and algorithms to ensure that the application is not only functional but also intuitive and responsive. This technological approach allows for real-time updates and feedback, which are essential for users who require consistent support and motivation. The inclusion of educational resources and direct links to professional help within the application further enriches the user's journey towards recovery.

The significance of our project extends to its potential impact on families and communities. By providing a tool that supports recovery and promotes understanding, we foster a more compassionate environment where individuals struggling with addiction are met with support rather than stigma. This shift in dynamics can significantly amplify the overall health and harmony within communities, making our application a valuable asset in the ongoing battle against drug abuse and addiction.

## Installation And Instruction To Use

### Installation
**For Windows and macOS:**
1. Ensure Python 3.8 or higher is installed on your system. You can download it from [python.org](https://www.python.org/downloads/).
2. Our application is designed to operate using Python's standard library, it is not necessary to install any external libraries, simplifying setup and maintenance.
   
4. Clone the repository:
   ```bash
   git clone git@github.com:Kunj-13/Recovery-Tracker.git
   cd Recovery-Tracker
   ```
  
### Instructions to Use
1. Start the application by running the main script. Make sure you are still in the project's root directory:
   ```bash
   python main.py
   ```
  This command will start the application in the command line interface.

2. Using the application:
- **Register or Log In**: Follow the prompts to register as a new user or log in with existing credentials.
- **Navigate through the application:** Use the command line options to access different features such as adding milestones, updating personal information, or adding journal entries.
- **Journal and Milestones:** Enter your daily experiences and track significant achievements as part of your recovery process.
- **Health Metrics**: Regularly update and review health metrics as prompted by the application.

## Structure of the Code

Our application is structured around four main Python modules, each serving distinct roles within the system:

1. **admin_module.py**
- Purpose: Handles administrative functions related to user management.
**Functions:**
- register_user(): Registers a new user with their credentials and personal details.
- display_users(): Lists all registered users.
- list_entries(): Shows all journal entries for a specific user.
2. **shared_functions.py**
- Purpose: Provides utility functions that are used across the application.
**Functions**:
- hash_password(): Secures passwords by hashing them before storage.
- read_credentials(), write_credentials(): Manages reading and writing user credentials to a file.
3. **main.py**
- Purpose: Acts as the entry point for the application, orchestrating user interactions and managing the application flow.
**Main Functionality:**
- Initiates the user interface.
- Calls functions from other modules based on user input.
4. **user_module.py**
- Purpose: Manages functionalities specific to the user's personal data and recovery tracking.
**Functions:**
- update_user_info(): Updates personal information of the user.
- add_personal_data(): Adds data related to the user’s recovery process.
  
### Interaction Between Modules
**Data Flow:** main.py serves as the controller that uses functions from admin_module.py and user_module-3.py to handle data input and operations. All modules interact with shared_functions.py for data management and utility operations like hashing.
**User Commands:** Users interact primarily through main-8.py, which directs commands to appropriate modules based on the operation (e.g., registering a user, adding journal entries).

## Functionalities and Test Results
Our Recovery Tracker application is designed to be an interactive tool for users and administrators to monitor and manage the recovery process from drug abuse and addiction. Below is an extensive overview of the application's functionalities and the test results to verify its performance.

## 1. Admin Login
### Test Procedure:
Log in as an admin. Select "View User Info" from the admin menu.
Enter the username of the account you wish to view.

### Expected Result:
The selected user's information is displayed, including username, email, and age.

<img width="378" alt="Screenshot 2024-04-15 at 10 35 24 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/a7061cea-f774-42d1-a0ca-27e1362668b5">

### Backend Operation:
**Admin_view_user_info()** function in **admin_module.py** retrieves and displays the user's details from the stored credentials.

## 1.1 Admin Actions
After the Admin logs in, it opens a whole new door of our application. It allows users to perform several functions such as:-

### Create a new user
When Admin presses 1, it allows the admin to create a user after entering all of the new users information.

<img width="372" alt="Screenshot 2024-04-15 at 10 42 19 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/ae7c6141-d04a-4ffc-8c5a-57efcb0652d5">

### View User info
When Admin presses option 2, our application provides admin with all the users names in our system they want to see their information of. After entering a certain user, it provides full list of all of that user's information. 

<img width="408" alt="Screenshot 2024-04-15 at 10 43 46 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/42dff422-203d-4ce1-ab99-d533645502d6">

### Delete a User
When the Admin selects the option 3, it allows them to delete a certain user after entering the information of the user they want to delete. 

<img width="522" alt="Screenshot 2024-04-15 at 10 51 00 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/286a3d9c-66fd-491a-bf15-15fc661795d8">

### View User Journals
When the Admin selects the option 4, the application allows the user to see any specific diary entry from any users in our system.

<img width="926" alt="Screenshot 2024-04-15 at 10 54 34 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/856c7ea8-49b1-4435-9df1-f409b5744b68">

### Logout
After performing all the desired actions, the Admin can select option 5 to logout of the system.

<img width="232" alt="Screenshot 2024-04-15 at 10 56 34 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/f87d91c3-6186-4213-80d0-cbd8fe796e57">

## 2. New User

### Test Procedure:
Run the Recovery Tracker application. Choose "New User" to initiate the registration process. Input the required details for username, email, age, and password. Also, when you are typing the password no one can see what you are typing for secuirty reasons so type carefully.

<img width="376" alt="Screenshot 2024-04-15 at 10 10 36 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/65776c12-cb45-4f38-ac81-8ca1a0d5a727">
<img width="386" alt="Screenshot 2024-04-15 at 10 29 48 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/a80524e4-5b50-4c8e-9b06-37d17ce44fe6">
<img width="692" alt="Screenshot 2024-04-15 at 10 31 09 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/c8ee6e03-7fe5-4a7f-9c5d-c519d195276e">


### Expected Result:
A new user account is created with the given details.
A confirmation message is displayed upon successful registration.

### Backend Operation:
**Register_user()** function in **Shared_functions.py** is invoked, which adds the new user to the credentials after validating the input and ensuring uniqueness.

## 3. Returning Users

### 3.1 Write New Entry
Allows users to write and save a new journal entry documenting their daily experiences, feelings, and progress.

**Instrutions:**
- Run the Recovery Tracker application.
- Select "Returning User" and log in with your credentials.
- Choose "Write new entry" by entering 1 from the user menu.
- Input the title, your current mood, and the content of your journal entry when prompted.

<img width="902" alt="Screenshot 2024-04-15 at 1 46 46 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/fa333c92-96ea-4f25-8d1e-cb6e209d31a7">
<img width="335" alt="Screenshot 2024-04-15 at 1 46 57 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/2e7992ed-1946-48ae-a9c4-92814cfe7945">

**Expected Result:**
- A new journal entry is created under your username with the provided details. A confirmation message "Journal entry saved" is displayed.

**Backend Operation:**
- The **write_entry()** function in **user_module.py** is called. This function prompts for entry details and appends the information to a text file representing the user's journal for the current date.

### 3.2 Read an entry
It allows users to retrieve and read journal entries from a specific date.

**Instructions:**
- After logging in, select "Read an entry" by entering 2 from the user menu.
- Enter the date of the journal entry you wish to read in the specified format.

![image](https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/0e7bf633-2085-42bb-aa8c-e910def30391)

**Expected Result:**
- The content of the journal entry for the given date is displayed. If no entry exists for that date, a message stating "No entries found for this date" is shown.

**Backend Operation:**
- The **read_entry()** function searches the user's journal directory for an entry file matching the date provided and displays its contents if found.

### 3.3 View Mood Statistics

**Instructions:**
- From the main menu, select "View mood statistics" by entering 3 after logging in.
- The application will process and display statistics without any additional input.
  
<img width="492" alt="Screenshot 2024-04-15 at 4 33 33 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/34ce43d5-b53d-4cc8-9725-a8a891b2ab97">

**Expected Result:**
A summary of mood occurrences in your journal entries is displayed, such as "Happy: 5 time(s)".

**Backend Operation:**
**View_mood_statistics()** in **user_module.py** analyzes the mood information from all journal entries and provides a count of each mood type.

### 3.4 Search entries

**Instructions:**
Select "Search entries" by entering 4 and when prompted, input a keyword you would like to search for in your journal entries.

<img width="255" alt="Screenshot 2024-04-15 at 4 36 21 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/a2893b2f-9cce-4ef0-af8d-9a4aeedf3a57">
<img width="1042" alt="Screenshot 2024-04-15 at 4 36 48 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/f2e2acae-c720-4121-b02b-0837cb0f6c41">

**Expected Result:**
Entries containing the keyword are listed with their titles and dates.
If no entries contain the keyword, "No entries found with that keyword" is displayed.
**Backend Operation:**
**Search_entries()** looks through the user's journal entries for the keyword and displays each matching entry.

### 3.5 List all entries

**Instructions:**
Choose "List all entries" from the menu by entering 5. No additional input is needed.

<img width="393" alt="Screenshot 2024-04-15 at 4 42 24 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/e92f81a3-29e1-47c8-afc1-c8dd17f8a817">

**Expected Result:**
All journal entries for the user are listed by date and title.
**Backend Operation:**
**List_entries()** in **shared_functions.py** compiles a list of all journal entry filenames for the user, presenting them in an organized manner.

### 3.6 Delete an entry

**Instrutions:**
Log in and select "Delete an entry" by typing 6. You'll be prompted to enter the date of the entry you want to delete.

<img width="517" alt="Screenshot 2024-04-15 at 4 50 11 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/fde80a79-1bd5-4307-91af-175a90fb15f0">

**Expected Result:**
The specified entry is deleted, and "Entry for the specific date you entered is deleted" confirms the action.
**Backend Operation:**
**Delete_user_entry()** in **user_module.py** removes the specified file from the user's journal directory.

### 3.7 Delete your account

**Instructions:**
Inside the user menu, choose "Delete your account" and confirm your decision when prompted.
<img width="692" alt="Screenshot 2024-04-15 at 10 31 09 AM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/c8ee6e03-7fe5-4a7f-9c5d-c519d195276e">
<img width="372" alt="Screenshot 2024-04-15 at 5 00 38 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/cb6a40eb-4b30-4758-b36a-3b5d892761a1">
<img width="722" alt="Screenshot 2024-04-15 at 5 01 48 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/997e2c7c-a022-4438-8f37-2d6efc6e6ac9">

**Expected Result:**
The user's account and all associated data are permanently removed, with a message confirming the deletion.
**Backend Operation:**
**Delete_own_account()** from **user_module.py** erases the user's credentials and journal entries from the system.

### 3.8 Set Recovery Start Date

**Instruction:**
From the user options, select "Set Recovery Start Date" and input the date when prompted.

<img width="408" alt="Screenshot 2024-04-15 at 5 08 06 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/a744b76b-9cbd-470e-bf9b-5950665e983a">
<img width="640" alt="Screenshot 2024-04-15 at 5 08 23 PM" src="https://github.com/Kunj-13/Recovery-Tracker/assets/143433713/24be1928-cae0-45a7-833f-028ad1528e74">

**Expected Result:**
The user's recovery start date is updated in the system, with a confirmation message.
**Backend Operation:**
**Set_recovery_start_date()** updates the user's credentials with the specified start date for recovery tracking.

### 3.9 
## Discussion 
The development of the Recovery Tracker application has encountered several notable issues and limitations that need to be addressed. One primary concern is the application's data security and privacy measures, which rely on basic password hashing and leave the sensitive user information vulnerable to potential breaches. This challenge is closely tied to the course topic on Security and Protection. The team should explore more robust encryption and access control mechanisms to ensure the confidentiality and integrity of the user data.

Another limitation is the lack of comprehensive data visualization and reporting tools, which is related to File-System and I/O Systems. The current focus on data collection and storage does not provide users with the necessary insights to effectively interpret their recovery progress over time. By leveraging their understanding of file management and input/output systems, the team can incorporate interactive visualizations, trend analysis, and personalized insights to significantly enhance the application's value.

The application's lack of customization and personalization options, which offers a one-size-fits-all approach, is linked to the course topic on Distributed Systems. Enabling greater user customization and personalization would improve the application's user-friendliness and foster a stronger sense of ownership and engagement among the users. The team can apply their knowledge of distributed systems to develop a more flexible and adaptable application architecture that supports personalization features.
## Conclusion 
In the process of developing the Recovery Tracker application, the team has leveraged various course learnings from Tthis course, including topics related to Operating System Structure, File-System, I/O Systems, Security and Protection, and Distributed Systems. These course learnings have been instrumental in addressing the identified issues and limitations, enabling the team to transform the Recovery Tracker into a more comprehensive and effective tool for supporting individuals in their quest for long-term recovery and improved well-being.

Regarding Operating System Structure, the team's understanding of file management and offline functionality has been applied to enhance the application's resilience and accessibility, ensuring users can access the application and their data even in areas with limited internet connectivity. The team's knowledge of File-System and I/O Systems has been crucial in incorporating robust data visualization and reporting capabilities, empowering users to interpret their recovery progress more effectively. Additionally, the team's insights into Security and Protection have informed the development of more secure data storage and access control mechanisms, safeguarding the sensitive user information. Finally, the team's understanding of Distributed Systems has guided the creation of a flexible and adaptable application architecture, supporting greater customization and personalization options for users.
