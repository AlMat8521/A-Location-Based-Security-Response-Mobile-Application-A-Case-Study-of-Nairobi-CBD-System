<h1> Title: A Location-Based Security Response Mobile Application: A Case Study of Nairobi CBD </h1>

<strong> Author: Alan Maturu </strong>

<strong>  Degree: Master of Science in Information Technology </strong> 

<strong>  Institution: Strathmore University </strong> 

<strong> Date: June, 2024 </strong>


This thesis addresses the challenge of real-time reporting and response to security incidences in Nairobi, Kenya. It proposes a location-based mobile application to facilitate easy reporting of crimes to police stations and the assignment of on-duty officers to cases. The system aims to enhance accountability, transparency, and response times, leveraging GPS technology to manage real-time reporting, response, and criminal activity management within Nairobi. The study employs the Scrum methodology for agile development, ensuring continuous stakeholder engagement and improvement.

<h3> Introduction </h3>

The thesis explores the use of location-based technology for real-time crime reporting and response. It discusses the existing challenges in crime reporting and the limitations of current emergency response systems in Nairobi. The main objective is to develop a mobile system that improves the efficiency of crime reporting and response.

<h3> Literature Review </h3>

The literature review covers empirical studies on mobile systems and location-based services for security enhancement. It examines various technologies such as GPS, RFID, and cellular networks, and evaluates existing security applications and their impact on crime prevention and response.

<h3> Research Methodology </h3>

The study employs purposive sampling of Kenyan citizens and residents who have been victims of crime, along with police officers handling criminal cases. Data collection methods include surveys and system utilization by police officers. The Scrum methodology guides the system development, emphasizing stakeholder inclusion and iterative improvement.

<h3> Data Analysis </h3>

The data analysis section presents findings on the distribution of crime victims, preferred modes of crime reporting, and factors influencing the use of the mobile system. It highlights the system's impact on response times and user satisfaction.

<h3> System Design, Implementation, and Testing </h3>

This section details the system architecture, user interface design, and user roles. It covers the implementation of location-based functionality, system testing approaches, and results. The system demonstrates significant improvements in response times and case monitoring.

<h3> Conclusion and Recommendations </h3>

The conclusion summarizes the study's findings and provides recommendations for future work. It emphasizes the potential of location-based technology to transform crime reporting and response mechanisms in Nairobi.


<h3> How to Run the Code </h3>

<h4> Prerequisites: </h4>

Android Studio or Xcode for mobile development.

Node.js and npm for backend development.

PostgreSQL for database management.

Setup Instructions:

Clone the repository from GitHub.

`git clone https://github.com/AlanMaturu/SecurityResponseApp.git`

Navigate to the project directory and install dependencies:

`cd SecurityResponseApp`

Backup setup 

`npm install`

Set up the PostgreSQL database:

    Create a new database in PostgreSQL. You can use a tool like pgAdmin or the psql command-line tool:

    bash

createdb security_response_db

Update the config.js file with your PostgreSQL connection details:

javascript

    module.exports = {
      database: {
        host: 'localhost',
        port: 5432,
        user: 'your_username',
        password: 'your_password',
        database: 'security_response_db'
      }
    };

Run database migrations and seed data (if applicable):

bash

npm run migrate
npm run seed

Start the backend server:

bash

        npm start

    Mobile Application Setup:
        Android:
            Open Android Studio.
            Click on File > Open and navigate to the SecurityResponseApp/mobile/android directory.
            Sync the project with Gradle files.
            Run the application on an emulator or a physical Android device by clicking on the Run button or using the Shift + F10 shortcut.
        iOS:
            Open Xcode.
            Click on File > Open and navigate to the SecurityResponseApp/mobile/ios directory.
            Ensure you have a valid development team selected in Xcode settings.
            Run the application on an emulator or a physical iOS device by clicking on the Run button or using the Cmd + R shortcut.

Configuration

    API Endpoints:
        Ensure the mobile application is configured to communicate with the backend server.
        Update the API base URL in the mobile application's configuration file:

        javascript

    const API_BASE_URL = 'http://localhost:3000/api'; // Update with your server URL if different

Environment Variables:

    Create a .env file in the backend directory and add any necessary environment variables:

    bash

        PORT=3000
        DATABASE_URL=postgres://your_username:your_password@localhost:5432/security_response_db

Usage

    User Registration and Login:
        Open the mobile application.
        Register a new user account or log in with existing credentials.
        Ensure your account is verified and active.

    Reporting a Crime:
        Use the mobile application to report a crime by filling out the necessary forms.
        Attach any relevant details such as photos or descriptions.

    Monitoring and Response:
        As a law enforcement officer, log in to your account.
        Monitor the reported crimes and update the status as you respond to incidents.
        Use the real-time updates feature to keep users informed of the response progress.

Testing

    Unit Testing:
        Navigate to the backend directory:

        bash

cd backend

Run the unit tests:

bash

        npm test

    Functional Testing:
        Use tools like Postman to test API endpoints.
        Ensure all endpoints are functioning correctly by making requests and verifying the responses.

Deployment

    Deploying the Backend:
        Use a platform like Heroku, AWS, or DigitalOcean to deploy the backend server.
        Ensure the PostgreSQL database is accessible from the deployed server.
        Update the API base URL in the mobile application to point to the deployed backend server.

    Deploying the Mobile Application:
        Publish the Android application on Google Play Store.
        Publish the iOS application on Apple App Store.
        Ensure all necessary app store requirements are met and the application is thoroughly tested before publishing.

Contact Information

For any questions or further assistance, please contact Alan Maturu at alan.maturu@gmail.com.

