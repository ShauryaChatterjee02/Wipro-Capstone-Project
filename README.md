# TestAutomationHybridFramework
A robust Hybrid Test Automation Framework developed using Selenium WebDriver, TestNG, Java, Maven, and Jenkins following the Page Object Model (POM) design pattern.
This framework automates multiple web UI functionalities on the Test Automation Practice application, covering form validation, alerts, dropdowns, drag-and-drop operations, file handling, web tables, navigation flows, and advanced browser interactions. The project incorporates data-driven testing using Excel, detailed reporting through Extent Reports, centralized logging with Log4j2, and automated browser management using WebDriverManager.

# Key Features

* Hybrid Framework using Page Object Model (POM) and Data-Driven Testing
* Selenium WebDriver with TestNG for UI Automation
* Excel-Based Test Data Management using Apache POI
* Extent Reports with Automatic Screenshot Capture
* Log4j2 Logging for Execution Tracking and Debugging
* Cross-Browser Testing Support (Chrome & Edge)
* WebDriverManager for Automatic Driver Configuration
* Reusable Utility Classes for Waits, Screenshots, and JavaScript Actions
* Jenkins CI/CD Pipeline Integration for Automated Execution
* Scalable, Maintainable, and Industry-Standard Framework Design

# Project Overview

This project is a Hybrid Test Automation Framework built using Selenium WebDriver, TestNG, Java, and Maven. It follows the Page Object Model (POM) design pattern and incorporates Data-Driven Testing, Extent Reports, Log4j2 logging, WebDriverManager, and Jenkins CI/CD integration to deliver a scalable, maintainable, and industry-standard automation solution.

## Tech Stack

| Technology         | Purpose                         |
| ------------------ | ------------------------------- |
| Java 17            | Core Programming Language       |
| Selenium WebDriver | Web UI Automation               |
| TestNG             | Test Execution & Assertions     |
| Maven              | Build & Dependency Management   |
| WebDriverManager   | Automatic Driver Setup          |
| Apache POI         | Excel-Based Data-Driven Testing |
| Extent Reports     | HTML Test Reporting             |
| Log4j2             | Logging & Debugging             |
| Jenkins            | CI/CD Pipeline Automation       |

# Project Structure

```text
TestAutomationHybridFramework/
│
├── src/
│   ├── test/
│   │   ├── java/
│   │   │   ├── Base/
│   │   │   │   └── BaseTest.java
│   │   │   │
│   │   │   ├── Listeners/
│   │   │   │   └── TestListener.java
│   │   │   │
│   │   │   ├── Pages/
│   │   │   │   ├── AlertPage.java
│   │   │   │   ├── DatePickerPage.java
│   │   │   │   ├── DoubleClickPage.java
│   │   │   │   ├── DownloadFilesPage.java
│   │   │   │   ├── DragDropPage.java
│   │   │   │   ├── DropDownPage.java
│   │   │   │   ├── DynamicButtonPage.java
│   │   │   │   ├── FooterPage.java
│   │   │   │   ├── FormPage.java
│   │   │   │   ├── HiddenAjaxPage.java
│   │   │   │   ├── LabelsAndLinksPage.java
│   │   │   │   ├── MouseHoverPage.java
│   │   │   │   ├── NavigationPage.java
│   │   │   │   ├── PaginationWebTablePage.java
│   │   │   │   ├── ShadowDomPage.java
│   │   │   │   ├── SliderPage.java
│   │   │   │   ├── SvgPage.java
│   │   │   │   ├── TablePage.java
│   │   │   │   ├── TabsPage.java
│   │   │   │   └── UploadPage.java
│   │   │   │
│   │   │   ├── Tests/
│   │   │   │   ├── AlertTest.java
│   │   │   │   ├── DatePickerTest.java
│   │   │   │   ├── DoubleClickTest.java
│   │   │   │   ├── DownloadFilesTest.java
│   │   │   │   ├── DragDropTest.java
│   │   │   │   ├── DropDownTest.java
│   │   │   │   ├── DynamicButtonTest.java
│   │   │   │   ├── FooterTest.java
│   │   │   │   ├── FormTest.java
│   │   │   │   ├── HiddenAjaxTest.java
│   │   │   │   ├── LabelsAndLinksTest.java
│   │   │   │   ├── MouseHoverTest.java
│   │   │   │   ├── NavigationTest.java
│   │   │   │   ├── PaginationWebTableTest.java
│   │   │   │   ├── ShadowDomTest.java
│   │   │   │   ├── SliderTest.java
│   │   │   │   ├── SvgTest.java
│   │   │   │   ├── TableTest.java
│   │   │   │   ├── TabsTest.java
│   │   │   │   └── UploadTest.java
│   │   │   │
│   │   │   ├── Utilities/
│   │   │   └── TestData/
│   │
│   └── resources/
│       ├── config.properties
│       ├── FormData.xlsx
│       ├── log4j2.xml
│       ├── sample.txt
│       ├── sample1.txt
│       └── sample2.txt
│
├── reports/
│   └── ExtentReport_*.html
│
├── Screenshots/
│   └── Failed Test Screenshots
│
├── logs/
│   └── automation.log
│
├── test-output/
│   └── TestNG Reports
│
├── Jenkinsfile
├── pom.xml
└── testng.xml
```
# Running Tests

Execute the complete automation suite:

```bash
mvn test
```

Execute tests using the TestNG suite configuration:

```bash
mvn test -DsuiteXmlFile=testng.xml
```

Execute an individual test class:

```bash
mvn test -Dtest=AlertTest
```

The framework leverages `testng.xml` for centralized test execution and integrates `TestListener` for reporting, logging, and test lifecycle management.
