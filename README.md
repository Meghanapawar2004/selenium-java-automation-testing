# Selenium Java Automation Testing

## Project Overview

This project demonstrates web application test automation using Java, Selenium WebDriver, TestNG, and Maven. It follows the Page Object Model (POM) design pattern to organize page interactions and test logic into reusable components.

The project is intended for learning fundamental automation testing concepts and practicing common web application test scenarios.

## Technologies Used

- **Programming Language:** Java 17
- **Automation Tool:** Selenium WebDriver 4
- **Testing Framework:** TestNG
- **Build and Dependency Management:** Maven
- **Design Pattern:** Page Object Model (POM) with PageFactory
- **Browser:** Google Chrome

## Test Scenarios

The project contains automated tests for the following workflows:

### 1. Login Testing
- Open the login page.
- Enter valid login credentials.
- Submit the login form.
- Verify that login succeeds.

### 2. Logout Testing
- Open the application's navigation menu.
- Select the logout option.
- Verify that the user is logged out.

### 3. Product and Shopping Cart Testing
- Select the Sauce Labs Backpack product.
- Add the product to the shopping cart.
- Open the cart.
- Verify that the selected product is present.
- Log out of the application.

These scenarios describe the existing test flows; their actual results should be confirmed by running the test suite.

## Project Structure

```text
selenium-java-automation-testing/
├── Project_Demo/
│   ├── Execution.PNG
│   └── Project Structure.PNG
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/abarnaselenium/pages/
│   │           ├── BasePage.java
│   │           ├── HomePage.java
│   │           ├── LoginPage.java
│   │           └── ProductPage.java
│   └── test/
│       └── java/
│           └── com/abarnaselenium/tests/
│               ├── BaseTest.java
│               ├── LoginTest.java
│               └── ProductTest.java
├── pom.xml
├── testng.xml
├── .gitignore
├── LICENSE
└── README.md
```

## Framework Components

| Component | Purpose |
|---|---|
| `BasePage.java` | Contains reusable page-level utilities |
| `LoginPage.java` | Handles login page interactions |
| `HomePage.java` | Handles home page actions and logout |
| `ProductPage.java` | Handles product selection and cart verification |
| `BaseTest.java` | Manages WebDriver setup and teardown |
| `LoginTest.java` | Contains login-related test cases |
| `ProductTest.java` | Contains product and cart test cases |
| `testng.xml` | Defines the TestNG test suite |
| `pom.xml` | Defines dependencies and build configuration |

## Prerequisites

Before running the project, ensure you have:

- Java Development Kit (JDK) 17
- Maven installed, or Maven support in your IDE
- Google Chrome installed
- IntelliJ IDEA or Eclipse (recommended)

## How to Run the Project

### Option 1: Run from an IDE

1. Open the project in IntelliJ IDEA or Eclipse.
2. Allow Maven to download the required dependencies.
3. Verify that Java 17 is configured.
4. Locate `testng.xml`.
5. Run the TestNG suite.

### Option 2: Run using Maven

Open a terminal in the project root directory and execute:

```bash
mvn clean test
```

Maven will compile the project and run the configured tests.

## Test Execution and Results

After execution, review the test output to determine which tests passed or failed.

Maven Surefire reports are generally generated under:

```text
target/surefire-reports/
```

The repository also contains demonstration screenshots in the `Project_Demo/` directory.

Only report verified execution results. Actual test outcomes may vary depending on browser configuration, application availability, and test data.

## Key Learning Outcomes

- Understanding Selenium WebDriver fundamentals
- Creating automated tests using Java
- Organizing test code using the Page Object Model
- Using TestNG to execute test suites
- Managing dependencies with Maven
- Using waits and reusable page methods
- Verifying login and shopping cart workflows

## Future Enhancements

- Add negative login scenarios.
- Add data-driven testing using external test data.
- Integrate automated screenshot capture for failures.
- Add detailed HTML test reports.
- Integrate the test suite into a CI/CD pipeline.

## Disclaimer

This is an educational automation testing project. Review the source code, execute the tests, and document your own findings before presenting the project as personal work. Retain the original license and any required attribution for reused materials.
