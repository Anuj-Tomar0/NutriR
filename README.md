# NutriR

Nutrition Tracker Shiny App
Overview
The Nutrition Tracker Shiny App is an interactive web application designed to help users track their nutritional intake, calculate their Body Mass Index (BMI), determine their daily calorie requirements, upload nutritional data, and generate customized meal plans. The app leverages a nutrition dataset containing detailed information about food items, including calorie content, macro and micronutrients, and other health-related parameters.

With user authentication powered by Google, the app provides a seamless and secure experience. Whether you're looking to optimize your diet, manage your calorie intake, or build personalized meal plans, this app offers a powerful toolset to achieve your nutritional goals.

Features
Breakdown Nutritional Values: Users can enter food items and view a breakdown of the nutritional information, including calories, fats, proteins, carbohydrates, vitamins, and minerals.
BMI Calculation: Users can input their height and weight to calculate their BMI, a useful measure of body fat based on height and weight.
Calorie Requirement: Based on user input, the app calculates the required daily calorie intake for maintaining, gaining, or losing weight.
Custom Meal Plans: Users can generate meal plans that align with their dietary goals, ensuring proper nutrition and calorie balance.
Upload Nutritional Data: Users can upload their custom nutritional datasets in CSV format for analysis and meal planning.
Google Authentication: The app integrates Google authentication, allowing users to log in securely using their Google account.
Prerequisites
Before using the app, ensure you have the following prerequisites installed:

R (version 4.0 or higher)
Shiny (install via install.packages("shiny"))
shinymaterial (for enhanced UI components: install.packages("shinymaterial"))
shinymanager (for authentication: install.packages("shinymanager"))
googlesheets4 (for handling Google Sheets authentication: install.packages("googlesheets4"))
tidyverse (for data manipulation: install.packages("tidyverse"))
Additionally, ensure you have access to Google Sheets for authentication purposes and a Google Cloud project set up to enable Google authentication.

Installation
Clone the Repository
To get started with the app, clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/nutrition-tracker-shiny-app.git
cd nutrition-tracker-shiny-app
Install Dependencies
After cloning the repository, navigate to the app directory and install the required R packages by running the following command:

R
Copy code
install.packages(c("shiny", "shinymaterial", "shinymanager", "googlesheets4", "tidyverse"))
Google Authentication Setup
Set up a Google Cloud project.
Enable the Google Sheets API and generate OAuth 2.0 credentials.
Download the credentials JSON file and save it in the app directory.
In the global.R file, provide the path to your credentials JSON file for Google authentication.
R
Copy code
googlesheets4::gs4_auth(path = "path_to_your_credentials.json")
Running the App
To run the app locally, simply run the following command in R:

R
Copy code
shiny::runApp()
This will launch the app in your default web browser.

Functionality Walkthrough
Nutritional Breakdown
The app allows users to input food items and receive a detailed breakdown of their nutritional values. The key nutritional parameters displayed include:

Calories
Total Fat
Sodium
Carbohydrates
Fiber
Protein
Vitamins (A, C, D)
Minerals (Calcium, Iron, Potassium)
By inputting the food item name or selecting it from a dropdown menu, users can view the corresponding data in an easily understandable format.

BMI Calculation
Users can calculate their BMI by entering their height and weight into the designated fields. The app will compute their BMI and provide feedback on their health status (underweight, normal weight, overweight, obese).

Calorie Requirement
To help users manage their diet, the app computes daily calorie requirements based on their age, gender, weight, height, and activity level. The app uses standard formulas like the Harris-Benedict Equation to calculate the Basal Metabolic Rate (BMR) and Total Daily Energy Expenditure (TDEE).

Custom Meal Plans
Based on user preferences, goals, and dietary restrictions, the app can generate personalized meal plans. Users can specify whether they are aiming for weight loss, weight maintenance, or weight gain, and the app will suggest meals that align with their calorie and nutrient requirements.

Uploading Nutritional Data
The app allows users to upload their custom datasets in CSV format. The nutritional data in the file will be parsed and displayed within the app, enabling users to perform analysis and meal planning on their specific data.

Google Authentication
To ensure a secure and personalized experience, the app integrates Google authentication. Users can log in using their Google account, enabling access to saved meal plans and preferences. The Google authentication setup is handled by the shinymanager package.

How to Contribute
If you would like to contribute to the development of the Nutrition Tracker Shiny App, follow these steps:

Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.
Push your changes to your forked repository.
Create a pull request to merge your changes with the main repository.
Please make sure to follow proper coding standards and include tests for any new functionality you add.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Contact
For any questions or inquiries, feel free to open an issue on GitHub or contact the repository owner:

Author: Anuj
Email: anuj@example.com
GitHub: https://github.com/your-username
