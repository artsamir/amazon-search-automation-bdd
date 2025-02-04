# Amazon Search and Filter Automation
### This project is a Cucumber BDD Framework for automating search and filter functionality on Amazon's website. It includes scenarios for searching products, filtering by brands, iterating through a list of brands, and selecting random categories from a dropdown.
## Features
- Search for products
- Filter search results by brand
- Handle irrelevant search terms
- Iterate through a list of brands to filter search results
- Select random categories from the dropdown

## Tech Stack

This project uses the following technologies:

- ![Cucumber](https://img.shields.io/badge/Cucumber-%2304D100?logo=cucumber&logoColor=white) : For writing behavior-driven tests in Gherkin.
- ![Selenium](https://img.shields.io/badge/Selenium-%2300A3E0?logo=selenium&logoColor=white) : For browser automation and interaction with the Amazon website.
- ![Java](https://img.shields.io/badge/Java-%23FF0000?logo=java&logoColor=white) : The primary programming language for the framework.
- ![TestNG](https://img.shields.io/badge/TestNG-%23F05A28?logo=testng&logoColor=white) : For managing and running tests.



## Project Structure
- **pageObjects:** Contains the Page Object Model (POM) classes for Home, Search Result, and Brand Filter pages.
- **stepDefinition:** Contains the step definitions for the Cucumber scenarios.
- **features:** Contains the feature files defining the scenarios. <br>
  ![image](https://github.com/user-attachments/assets/13af9473-a058-4bf7-a117-531a59f6d0d9)
  <br>


## Prerequisites
- Java JDK (1.8 or higher)
- Maven (3.6.0 or higher)
- ChromeDriver (Ensure compatibility with your Chrome browser version)
## Setup Instructions
 1. Clone the repository:
 git clone (https://github.com/artsamir/Alphabin_Assignment.git) <br>
 cd Alphabin_Assignment
 2. Install dependencies: mvn clean install
 3. Run the tests: mvn test

# Project Components
## Page Objects
- **HomePage:** Contains methods to interact with the Amazon homepage.
- **SearchResultPage:** Contains methods to interact with the search results page.
- **BrandFilterPage:** Contains methods to interact with the brand filter section.

## Step Definition
- **AmazonSteps:** Contains the implementation of the steps defined in the feature files.
## Feature Files
- **amazonSearch.feature:** Contains the scenarios for testing search and filter functionality on Amazon.
 <br>

  ![image](https://github.com/user-attachments/assets/0b8ddcbf-8cf1-44e6-9d0d-5b9be234be1d)
<br>

# Test Case Execution result 
**Test Case 1 :** Search and Filter Functionality<br>
**Description :** To verify Search for Product and Filter by Brand<br>
**Test Step :**
    <br>
- Open The Application in Browser
- Search for "Wireless Headphones"
- Verify The Serach Result Containning "Wireless Headphones"
- In Filter section select "Sony" Brand
- Verify "Sony Wireless headphones" displayed
  <br>
  **Status :** Pass
  
**Test Case 2 :** Search Functionality<br>
**Description :** To verify Search With Irrelevent Term<br>
**Test Step :**
    <br>
- Open The Application in Browser
- Search for "Random Irrelevent keywords"
- Verify The Serach Result Should be less than 10 products
  <br>
  **Status :** Pass

**Test Case 3 :** Filter Functionality<br>
**Description :** To verify iterate through a list of brands and filter <br>
**Test Step :**
    <br>
- Open The Application in Browser
- Search for "Laptops"
- Verify The Serach Result Should be contain laptops
- Create a list of brands:["Apple","Dell","HP"] and Filter search results by iterating through brands in the list
- Verify the serach result displayed Specified brands for each iteration
  <br>
  **Status :** Pass

  **Test Case 4 :**  Category Dropdown Functionality<br>
**Description :** To verify in Category Dropdown Select any option Randomly and check Search result displayed with specified category<br>
**Test Step :**
    <br>
- Open The Application in Browser
- Collect all the category from dropdown and store in Array
- Randomly select a category from the Array
- The search result should be displayed choosen category
  <br>
**Status :**
> !Note
> Not able to assert properly 
  
# How to Run
1. Ensure Chromebrowser installed and ChromeDriver is in your path
2. Run the test using Maven: mvn test
   **This will execute all the 4 Scenarios**
   <br>
   ![image](https://github.com/user-attachments/assets/3fcab045-5156-42d6-96d2-dd299e0db2d9)
   <br>
   ![image](https://github.com/user-attachments/assets/21ae76dc-cfed-4d9d-91f1-466b7ccbeb34)
   <br>
   ![image](https://github.com/user-attachments/assets/4f4b2752-595d-40fc-933a-fb970c84f2fd)
   <br>


### Note:
- Parallel testing functionality
- Cross-browser capable <br> not done this part left.
