# Amazon Search and Filter Automation
### This project is a Cucumber BDD Framework for automating search and filter functionality on Amazon's website. It includes scenarios for searching products, filtering by brands, iterating through a list of brands, and selecting random categories from a dropdown.
## Features
- Search for products
- Filter search results by brand
- Handle irrelevant search terms
- Iterate through a list of brands to filter search results
- Select random categories from the dropdown

## Project Structure
- **pageObjects:** Contains the Page Object Model (POM) classes for Home, Search Result, and Brand Filter pages.
- **stepDefinition:** Contains the step definitions for the Cucumber scenarios.
- **features:** Contains the feature files defining the scenarios.

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

# How to Run
1. Ensure Chromebrowser installed and ChromeDriver is in your path
2. Run the test using Maven: mvn test
   **This will execute all the 4 Scenarios**

### Note: Sorry.. for Not completed the Assignment properly. More time spent in this project filtering part. 
- Parallel testing functionality
- Cross-browser capable <br> not done this part left.
