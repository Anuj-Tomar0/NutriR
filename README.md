# Nutrition Tracker Shiny App

## Overview

The **Nutrition Tracker Shiny App** is an interactive web application designed to help users track their nutritional intake, calculate their Body Mass Index (BMI), determine their daily calorie requirements, upload nutritional data, and generate customized meal plans. The app leverages a nutrition dataset containing detailed information about food items, including calorie content, macro and micronutrients, and other health-related parameters. 

With user authentication powered by **Google**, the app provides a seamless and secure experience. Whether you're looking to optimize your diet, manage your calorie intake, or build personalized meal plans, this app offers a powerful toolset to achieve your nutritional goals.

## Features

- **Breakdown Nutritional Values**: Users can enter food items and view a breakdown of the nutritional information, including calories, fats, proteins, carbohydrates, vitamins, and minerals.
- **BMI Calculation**: Users can input their height and weight to calculate their BMI, a useful measure of body fat based on height and weight.
- **Calorie Requirement**: Based on user input, the app calculates the required daily calorie intake for maintaining, gaining, or losing weight.
- **Custom Meal Plans**: Users can generate meal plans that align with their dietary goals, ensuring proper nutrition and calorie balance.
- **Upload Nutritional Data**: Users can upload their custom nutritional datasets in CSV format for analysis and meal planning.
- **Google Authentication**: The app integrates Google authentication, allowing users to log in securely using their Google account.

## Prerequisites

Before using the app, ensure you have the following prerequisites installed:

- **R** (version 4.0 or higher)
- **Shiny** (install via `install.packages("shiny")`)
- **shinymaterial** (for enhanced UI components: `install.packages("shinymaterial")`)
- **shinymanager** (for authentication: `install.packages("shinymanager")`)
- **googlesheets4** (for handling Google Sheets authentication: `install.packages("googlesheets4")`)
- **tidyverse** (for data manipulation: `install.packages("tidyverse")`)

Additionally, ensure you have access to Google Sheets for authentication purposes and a Google Cloud project set up to enable Google authentication.

## Installation

### Clone the Repository

To get started with the app, clone the repository to your local machine:

```bash
git clone https://github.com/your-username/nutrition-tracker-shiny-app.git
cd nutrition-tracker-shiny-app
