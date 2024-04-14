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

## Discussion and Conclusions
## Strengths
### Comprehensive Approach to Recovery Support
- The application provides a well-rounded set of features, including personal milestone tracking, health metrics visualization, journaling, and access to educational resources, to support users in their recovery journey.
### User-Centric Design
- The project emphasizes user-friendliness and privacy, making the application accessible to users of various technological backgrounds.
### Leveraging Data Structures and Algorithms
- The project utilizes appropriate data structures and algorithms to store and manage user data efficiently, enhancing the application's functionality and responsiveness.
## Limitations and Potential Improvements
### Data Security and Encryption
- The application could benefit from additional data encryption measures to protect the integrity and confidentiality of sensitive user information.
### Visualization and Analytics
- Enhancing the data visualization capabilities, such as graphs and trend analysis, could help users better understand their recovery patterns and progress.
### Connectivity and Integration
- Incorporating features that allow users to connect with support groups, healthcare providers, or other recovery resources could further enhance the application's value and user experience.
## Application of Course Learnings
### Data Structures and Algorithms
- The project utilizes appropriate data structures and algorithms to store and manage user data efficiently.
### Modular Design
- The separation of concerns into distinct modules promotes code maintainability, testability, and scalability.
### User Interface and Experience
- The project emphasizes user-friendliness and accessibility, demonstrating the application of UI/UX design best practices.

