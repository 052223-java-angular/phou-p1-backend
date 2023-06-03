# Yield - A P&L generator for your trades

## Introduction

Yield is an web application that allows a user to upload a .csv file of their trades and generate a profit and loss .csv report. In addition to generating a
.csv report, the user can view the generated results within a web-browser like Chrome.

As part of the integration, yield will utilize the Coinmarketcap or similar API to extract past and current price data of crypto assets for calculating figures.

Although the app is free to use, yield may also integrate the Coinbase API for accepting crypto payment / donations for those feeling the need to donate some of
those Gainz!

## BE User Stories

- **As a user**, I want to be able to register and login, so I can save my reports and retrieve those reports at a later time.
- **As a user**, I want to be able to retrieve my trades and generate a report in .csv or .json format.
- **As a user**, I want to be able to query and retrieve my reports by asset, date, amount.

## MVP (Minimum Viable Product)

- User registration
- User login via jwt authentication
- Adding and modifying trade / order history
- Generating P&L report and sending the report back the user in .csv and / or .json format
- Search and query for trade records by asset, date and amount
- Fetching cryptocurrency prices from coinmarket or coingecko or other API

## Stretch Goals

- Add asynchronous processing for fetching API data
- Add send report by email
- Implement threads in order to increase processing times for generating reports

## Tech Stack

### **Back-end tech stack**

- **Java**: The main programming language used for building the application.
- **PostgreSQL**: Used as the database to store user reports and cryptocurrency related data.
- **JDBC (Java Database Connectivity)**: An API for connecting and executing queries on the database.
- **Maven or Gradle**: Used for managing project dependencies.
- **BCrypt**: A Java library for hashing and checking passwords for security.
- **Log4j**: A logging utility for debugging purposes.
- **JUnit**: A testing framework for Java applications, used to ensure our code works as expected.
- **JUnit, Mockito, and PowerMock**: Used for unit and integration testing.
- **Git and GitHub**: Used for version control.

## Requirements

- **Clean Codebase**: All code should be clean and well-documented. The repository should not include any unnecessary files or folders such as the `target/`,
  `.DS_Store`, etc. All files and directories should be appropriately named and organized.

- **Database Design**: The database should be designed following the principles of the 3rd Normal Form (3NF) to ensure data integrity and efficiency. An Entity
  Relationship Diagram (ERD) should be included in the documentation.

- **Secure**: All sensitive user data such as passwords must be securely hashed before storing it in the database. The application should not display any
  sensitive information in error messages.

- **Error Handling**: The application should handle potential errors gracefully and provide clear and helpful error messages to the users.

- **Testing**: The application should have a high test coverage. Unit tests and integration tests should be implemented using JUnit, Mockito, and PowerMock.

- **Version Control**: The application should be developed using a version control system, preferably Git, with regular commits denoting progress.

- **Documentation**: The repository should include a README file with clear instructions on how to run the application. Code should be well-commented to allow
  for easy understanding and maintenance.

- **Scalable**: The design of the application should be scalable, allowing for easy addition of new features or modifications in the future.
