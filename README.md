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

# Screenshots
## Jenkins Pipeline
<img width="1904" height="986" alt="Screenshot 2026-06-10 195401" src="https://github.com/user-attachments/assets/5b4a1199-d1ac-4a5d-8a75-a4e5bc51c67e" />

# Jenkins Console
<img width="1918" height="988" alt="Screenshot 2026-06-10 200115" src="https://github.com/user-attachments/assets/e7a4d2d2-1b61-42ba-a900-e8dfecc38814" />

# Date Picker
<img width="1544" height="506" alt="Screenshot 2026-06-10 200440" src="https://github.com/user-attachments/assets/775b0c02-d2e7-4725-b636-f610b20b04ce" />
<img width="1899" height="979" alt="Screenshot 2026-06-10 200340" src="https://github.com/user-attachments/assets/49b07e79-d144-4973-9512-d74d5ab90b50" />

# Multiple File Upload
<img width="1897" height="947" alt="Screenshot 2026-06-10 200650" src="https://github.com/user-attachments/assets/c452fd97-c6d7-4d80-aafb-d8dadac96d65" />
<img width="1542" height="460" alt="Screenshot 2026-06-10 200619" src="https://github.com/user-attachments/assets/6b21a4cc-3b42-486a-9569-0ebfd33e76a1" />

# AutomationSuite Test Execution Summary
<img width="1536" height="497" alt="Screenshot 2026-06-10 201411" src="https://github.com/user-attachments/assets/ad301bee-ee34-412c-9c30-3e0d88f4a4e4" />

# CI/CD Workflow

```text id="0if0zm"
GitHub Push
      ↓
Jenkins Pipeline
      ↓
Source Code Checkout
      ↓
Maven Build
      ↓
TestNG Test Execution
      ↓
Extent Report Generation
      ↓
TestNG Report Publishing
      ↓
Artifact Archiving
      ↓
Build Status
```
# Author

## Shaurya Chattopadhyay

### Automation Concepts Used

* Selenium WebDriver for Web UI Automation
* TestNG for Test Execution and Reporting
* Page Object Model (POM) for Maintainable Test Design
* Data-Driven Testing using Apache POI and Excel
* Jenkins CI/CD for Automated Build and Test Execution
* Extent Reports and Log4j2 for Reporting and Logging

# Extent Reports
[ExtentReport_20260610_200726.html](https://github.com/user-attachments/files/28800486/ExtentReport_20260610_200726.html)


<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<title>Automation Execution Report</title>
<link rel="apple-touch-icon" href="https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@b00a2d0486596e73dd7326beacf352c639623a0e/commons/img/logo.png">
<link rel="shortcut icon" href="https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@b00a2d0486596e73dd7326beacf352c639623a0e/commons/img/logo.png">
<link href="https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@ce8b10435bcbae260c334c0d0c6b61d2c19b6168/spark/css/spark-style.css" rel="stylesheet" />
<link href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@7cc78ce/spark/js/jsontree.js"></script>
<style type="text/css"></style></head><body class="spa -report standard">
  <div class="app">
    <div class="layout">
<div class="header navbar">
<div class="vheader">
<div class="nav-logo">
<a href="#">
<div class="logo" style="background-image: url('https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@b00a2d0486596e73dd7326beacf352c639623a0e/commons/img/logo.png')"></div>
</a>
</div>
<ul class="nav-left">
<li class="search-box">
<a class="search-toggle" href="#">
<i class="search-icon fa fa-search"></i>
<i class="search-icon-close fa fa-close"></i>
</a>
</li>
<li class="search-input"><input id="search-tests" class="form-control" type="text" placeholder="Search..."></li>
</ul>
<ul class="nav-right">
<li class="m-r-10">
<a href="#"><span class="badge badge-primary">Test Automation Hybrid Framework Report</span></a>
</li>
<li class="m-r-10">
<a href="#"><span class="badge badge-primary">Jun 10, 2026 08:07:26 PM</span></a>
</li>
</ul>
</div>
</div><div class="side-nav">
<div class="side-nav-inner">
<ul class="side-nav-menu">
<li class="nav-item dropdown" onclick="toggleView('test-view')">
<a id="nav-test" class="dropdown-toggle" href="#">
<span class="ico"><i class="fa fa-list"></i></span>
</a>
</li>
<li class="nav-item dropdown" onclick="toggleView('exception-view')">
<a id="nav-exception" class="dropdown-toggle" href="#">
<span class="ico"><i class="fa fa-bug"></i></span>
</a>
</li>
<li class="nav-item dropdown" onclick="toggleView('dashboard-view')">
<a id="nav-dashboard" class="dropdown-toggle" href="#">
<span class="ico"><i class="fa fa-bar-chart"></i></span>
</a>
</li>
</ul>
</div>
</div>      <div class="vcontainer">
        <div class="main-content">
<div class="test-wrapper row view test-view">
  <div class="test-list">
    <div class="test-list-tools">
<ul class="tools pull-left">
<li><a href="#"><span class="font-size-14">Tests</span></a></li>
</ul>
<ul class="tools text-right">
<li class="dropdown">
<a href="#" class="dropdown-toggle" data-toggle="dropdown"><i class="fa fa-exclamation-circle"></i></a>
<ul id="status-toggle" class="dropdown-menu dropdown-md p-v-0">
<a class="dropdown-item" status="pass" href="#"><span>Pass</span><span class="status success"></span></a>
<a class="dropdown-item" status="fail" href="#"><span>Fail</span><span class="status danger"></span></a>
<div class="dropdown-divider"></div>
<a status="clear" class="dropdown-item" href="#"><span>Clear</span><span class="pull-right"><i class="fa fa-close"></i></span></a>
</ul>
</li>
</ul>
</div>    <div class="test-list-wrapper scrollable">
      <ul class="test-list-item">
        <li class="test-item"  status="pass" test-id="1"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifySimpleAlert</p>
            <p class="text-sm">
              <span>8:07:32 PM</span> / <span>00:00:00:135</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifySimpleAlert</h5>
<span class='badge badge-success'>06.10.2026 8:07:32 PM</span>
<span class='badge badge-danger'>06.10.2026 8:07:32 PM</span>
<span class='badge badge-default'>00:00:00:135</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=1</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:07:32 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="2"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyConfirmationAccept</p>
            <p class="text-sm">
              <span>8:07:37 PM</span> / <span>00:00:00:137</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyConfirmationAccept</h5>
<span class='badge badge-success'>06.10.2026 8:07:37 PM</span>
<span class='badge badge-danger'>06.10.2026 8:07:37 PM</span>
<span class='badge badge-default'>00:00:00:137</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=2</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:07:37 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="3"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyConfirmationDismiss</p>
            <p class="text-sm">
              <span>8:07:42 PM</span> / <span>00:00:00:135</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyConfirmationDismiss</h5>
<span class='badge badge-success'>06.10.2026 8:07:42 PM</span>
<span class='badge badge-danger'>06.10.2026 8:07:42 PM</span>
<span class='badge badge-default'>00:00:00:135</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=3</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:07:42 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="4"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyPromptAlert</p>
            <p class="text-sm">
              <span>8:07:48 PM</span> / <span>00:00:00:141</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyPromptAlert</h5>
<span class='badge badge-success'>06.10.2026 8:07:48 PM</span>
<span class='badge badge-danger'>06.10.2026 8:07:48 PM</span>
<span class='badge badge-default'>00:00:00:141</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=4</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:07:48 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="5"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyPopupWindow</p>
            <p class="text-sm">
              <span>8:07:55 PM</span> / <span>00:00:01:964</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyPopupWindow</h5>
<span class='badge badge-success'>06.10.2026 8:07:55 PM</span>
<span class='badge badge-danger'>06.10.2026 8:07:57 PM</span>
<span class='badge badge-default'>00:00:01:964</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=5</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:07:57 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="6"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">testAllDatePickers</p>
            <p class="text-sm">
              <span>8:08:03 PM</span> / <span>00:00:00:710</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">testAllDatePickers</h5>
<span class='badge badge-success'>06.10.2026 8:08:03 PM</span>
<span class='badge badge-danger'>06.10.2026 8:08:03 PM</span>
<span class='badge badge-default'>00:00:00:710</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=6</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:08:03 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="7"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">testDoubleClickCopyText</p>
            <p class="text-sm">
              <span>8:08:08 PM</span> / <span>00:00:00:241</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">testDoubleClickCopyText</h5>
<span class='badge badge-success'>06.10.2026 8:08:08 PM</span>
<span class='badge badge-danger'>06.10.2026 8:08:08 PM</span>
<span class='badge badge-default'>00:00:00:241</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=7</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:08:08 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="8"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">automateDownloadFiles</p>
            <p class="text-sm">
              <span>8:08:13 PM</span> / <span>00:00:16:857</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">automateDownloadFiles</h5>
<span class='badge badge-success'>06.10.2026 8:08:13 PM</span>
<span class='badge badge-danger'>06.10.2026 8:08:30 PM</span>
<span class='badge badge-default'>00:00:16:857</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=8</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:08:30 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="9"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">testDragAndDrop</p>
            <p class="text-sm">
              <span>8:08:35 PM</span> / <span>00:00:00:333</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">testDragAndDrop</h5>
<span class='badge badge-success'>06.10.2026 8:08:35 PM</span>
<span class='badge badge-danger'>06.10.2026 8:08:35 PM</span>
<span class='badge badge-default'>00:00:00:333</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=9</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:08:35 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="10"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyDropDown</p>
            <p class="text-sm">
              <span>8:08:41 PM</span> / <span>00:00:23:729</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyDropDown</h5>
<span class='badge badge-success'>06.10.2026 8:08:41 PM</span>
<span class='badge badge-danger'>06.10.2026 8:09:04 PM</span>
<span class='badge badge-default'>00:00:23:729</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=10</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:09:04 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="11"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyStartStopStartButton</p>
            <p class="text-sm">
              <span>8:09:10 PM</span> / <span>00:00:04:276</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyStartStopStartButton</h5>
<span class='badge badge-success'>06.10.2026 8:09:10 PM</span>
<span class='badge badge-danger'>06.10.2026 8:09:14 PM</span>
<span class='badge badge-default'>00:00:04:276</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=11</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:09:14 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="fail" test-id="12"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">testFooterLinks</p>
            <p class="text-sm">
              <span>8:09:19 PM</span> / <span>00:00:20:703</span>
              <span class="badge fail-bg log float-right">Fail</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-fail">testFooterLinks</h5>
<span class='badge badge-success'>06.10.2026 8:09:19 PM</span>
<span class='badge badge-danger'>06.10.2026 8:09:40 PM</span>
<span class='badge badge-default'>00:00:20:703</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=12</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log fail-bg">Fail</span></td>
        <td>8:09:40 PM</td>
        <td>
          <textarea readonly class="code-block">java.lang.IndexOutOfBoundsException: Index 1 out of bounds for length 0
	at java.base/jdk.internal.util.Preconditions.outOfBounds(Preconditions.java:64)
	at java.base/jdk.internal.util.Preconditions.outOfBoundsCheckIndex(Preconditions.java:70)
	at java.base/jdk.internal.util.Preconditions.checkIndex(Preconditions.java:266)
	at java.base/java.util.Objects.checkIndex(Objects.java:359)
	at java.base/java.util.ArrayList.get(ArrayList.java:427)
	at Pages.FooterPage.clickAllFooterLinks(FooterPage.java:33)
	at Tests.FooterTest.testFooterLinks(FooterTest.java:20)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at java.base/jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77)
	at java.base/jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.base/java.lang.reflect.Method.invoke(Method.java:568)
	at org.testng.internal.invokers.MethodInvocationHelper.invokeMethod(MethodInvocationHelper.java:141)
	at org.testng.internal.invokers.TestInvoker.invokeMethod(TestInvoker.java:687)
	at org.testng.internal.invokers.TestInvoker.invokeTestMethod(TestInvoker.java:230)
	at org.testng.internal.invokers.MethodRunner.runInSequence(MethodRunner.java:63)
	at org.testng.internal.invokers.TestInvoker$MethodInvocationAgent.invoke(TestInvoker.java:995)
	at org.testng.internal.invokers.TestInvoker.invokeTestMethods(TestInvoker.java:203)
	at org.testng.internal.invokers.TestMethodWorker.invokeTestMethods(TestMethodWorker.java:154)
	at org.testng.internal.invokers.TestMethodWorker.run(TestMethodWorker.java:134)
	at java.base/java.util.ArrayList.forEach(ArrayList.java:1511)
	at org.testng.TestRunner.privateRun(TestRunner.java:741)
	at org.testng.TestRunner.run(TestRunner.java:616)
	at org.testng.SuiteRunner.runTest(SuiteRunner.java:421)
	at org.testng.SuiteRunner.runSequentially(SuiteRunner.java:413)
	at org.testng.SuiteRunner.privateRun(SuiteRunner.java:373)
	at org.testng.SuiteRunner.run(SuiteRunner.java:312)
	at org.testng.SuiteRunnerWorker.runSuite(SuiteRunnerWorker.java:52)
	at org.testng.SuiteRunnerWorker.run(SuiteRunnerWorker.java:95)
	at org.testng.TestNG.runSuitesSequentially(TestNG.java:1274)
	at org.testng.TestNG.runSuitesLocally(TestNG.java:1208)
	at org.testng.TestNG.runSuites(TestNG.java:1112)
	at org.testng.TestNG.run(TestNG.java:1079)
	at org.testng.remote.AbstractRemoteTestNG.run(AbstractRemoteTestNG.java:115)
	at org.testng.remote.RemoteTestNG.initAndRun(RemoteTestNG.java:293)
	at org.testng.remote.RemoteTestNG.main(RemoteTestNG.java:91)
</textarea>
          
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="13"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">testForm</p>
            <p class="text-sm">
              <span>8:09:44 PM</span> / <span>00:00:06:723</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">testForm</h5>
<span class='badge badge-success'>06.10.2026 8:09:44 PM</span>
<span class='badge badge-danger'>06.10.2026 8:09:51 PM</span>
<span class='badge badge-default'>00:00:06:723</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=13</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:09:51 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="14"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">automateHiddenAjax</p>
            <p class="text-sm">
              <span>8:09:56 PM</span> / <span>00:00:08:666</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">automateHiddenAjax</h5>
<span class='badge badge-success'>06.10.2026 8:09:56 PM</span>
<span class='badge badge-danger'>06.10.2026 8:10:04 PM</span>
<span class='badge badge-default'>00:00:08:666</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=14</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:10:04 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="15"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyLabelsAndLinks</p>
            <p class="text-sm">
              <span>8:10:10 PM</span> / <span>00:01:23:429</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyLabelsAndLinks</h5>
<span class='badge badge-success'>06.10.2026 8:10:10 PM</span>
<span class='badge badge-danger'>06.10.2026 8:11:33 PM</span>
<span class='badge badge-default'>00:01:23:429</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=15</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:11:33 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="16"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyMouseHover1</p>
            <p class="text-sm">
              <span>8:11:38 PM</span> / <span>00:00:00:397</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyMouseHover1</h5>
<span class='badge badge-success'>06.10.2026 8:11:38 PM</span>
<span class='badge badge-danger'>06.10.2026 8:11:38 PM</span>
<span class='badge badge-default'>00:00:00:397</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=16</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:11:38 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="17"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyMouseHover2</p>
            <p class="text-sm">
              <span>8:11:44 PM</span> / <span>00:00:00:380</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyMouseHover2</h5>
<span class='badge badge-success'>06.10.2026 8:11:44 PM</span>
<span class='badge badge-danger'>06.10.2026 8:11:45 PM</span>
<span class='badge badge-default'>00:00:00:380</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=17</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:11:45 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="18"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyHomeNavigation</p>
            <p class="text-sm">
              <span>8:11:50 PM</span> / <span>00:00:05:347</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyHomeNavigation</h5>
<span class='badge badge-success'>06.10.2026 8:11:50 PM</span>
<span class='badge badge-danger'>06.10.2026 8:11:55 PM</span>
<span class='badge badge-default'>00:00:05:347</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=18</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:11:55 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="19"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyUdemyCoursesNavigation</p>
            <p class="text-sm">
              <span>8:12:02 PM</span> / <span>00:00:07:849</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyUdemyCoursesNavigation</h5>
<span class='badge badge-success'>06.10.2026 8:12:02 PM</span>
<span class='badge badge-danger'>06.10.2026 8:12:10 PM</span>
<span class='badge badge-default'>00:00:07:849</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=19</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:12:10 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="20"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyOnlineTrainingsNavigation</p>
            <p class="text-sm">
              <span>8:12:14 PM</span> / <span>00:00:05:948</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyOnlineTrainingsNavigation</h5>
<span class='badge badge-success'>06.10.2026 8:12:14 PM</span>
<span class='badge badge-danger'>06.10.2026 8:12:20 PM</span>
<span class='badge badge-default'>00:00:05:948</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=20</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:12:20 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="21"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyBlogNavigation</p>
            <p class="text-sm">
              <span>8:12:25 PM</span> / <span>00:00:04:950</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyBlogNavigation</h5>
<span class='badge badge-success'>06.10.2026 8:12:25 PM</span>
<span class='badge badge-danger'>06.10.2026 8:12:30 PM</span>
<span class='badge badge-default'>00:00:04:950</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=21</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:12:30 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="22"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyPlaywrightPracticeNavigation</p>
            <p class="text-sm">
              <span>8:12:35 PM</span> / <span>00:00:05:181</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyPlaywrightPracticeNavigation</h5>
<span class='badge badge-success'>06.10.2026 8:12:35 PM</span>
<span class='badge badge-danger'>06.10.2026 8:12:40 PM</span>
<span class='badge badge-default'>00:00:05:181</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=22</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:12:40 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="23"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyPaginationWebTable</p>
            <p class="text-sm">
              <span>8:12:46 PM</span> / <span>00:00:10:883</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyPaginationWebTable</h5>
<span class='badge badge-success'>06.10.2026 8:12:46 PM</span>
<span class='badge badge-danger'>06.10.2026 8:12:57 PM</span>
<span class='badge badge-default'>00:00:10:883</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=23</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:12:57 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="24"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyShadowDomElements</p>
            <p class="text-sm">
              <span>8:13:03 PM</span> / <span>00:00:00:422</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyShadowDomElements</h5>
<span class='badge badge-success'>06.10.2026 8:13:03 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:04 PM</span>
<span class='badge badge-default'>00:00:00:422</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=24</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:04 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="25"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifySliderMovement</p>
            <p class="text-sm">
              <span>8:13:11 PM</span> / <span>00:00:02:425</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifySliderMovement</h5>
<span class='badge badge-success'>06.10.2026 8:13:11 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:13 PM</span>
<span class='badge badge-default'>00:00:02:425</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=25</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:13 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="26"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifySVGElements</p>
            <p class="text-sm">
              <span>8:13:20 PM</span> / <span>00:00:03:073</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifySVGElements</h5>
<span class='badge badge-success'>06.10.2026 8:13:20 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:23 PM</span>
<span class='badge badge-default'>00:00:03:073</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=26</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:23 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="27"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyCellData</p>
            <p class="text-sm">
              <span>8:13:28 PM</span> / <span>00:00:00:027</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyCellData</h5>
<span class='badge badge-success'>06.10.2026 8:13:28 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:29 PM</span>
<span class='badge badge-default'>00:00:00:027</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=27</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:29 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="28"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyColumnCount</p>
            <p class="text-sm">
              <span>8:13:33 PM</span> / <span>00:00:00:016</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyColumnCount</h5>
<span class='badge badge-success'>06.10.2026 8:13:33 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:33 PM</span>
<span class='badge badge-default'>00:00:00:016</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=28</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:33 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="29"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyRowCount</p>
            <p class="text-sm">
              <span>8:13:38 PM</span> / <span>00:00:00:016</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyRowCount</h5>
<span class='badge badge-success'>06.10.2026 8:13:38 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:38 PM</span>
<span class='badge badge-default'>00:00:00:016</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=29</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:38 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="30"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifySearchInTable</p>
            <p class="text-sm">
              <span>8:13:43 PM</span> / <span>00:00:00:046</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifySearchInTable</h5>
<span class='badge badge-success'>06.10.2026 8:13:43 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:44 PM</span>
<span class='badge badge-default'>00:00:00:046</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=30</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:44 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="31"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyWikipediaSearch</p>
            <p class="text-sm">
              <span>8:13:48 PM</span> / <span>00:00:03:205</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyWikipediaSearch</h5>
<span class='badge badge-success'>06.10.2026 8:13:48 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:51 PM</span>
<span class='badge badge-default'>00:00:03:205</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=31</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:51 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="32"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifySingleFileUpload</p>
            <p class="text-sm">
              <span>8:13:57 PM</span> / <span>00:00:00:190</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifySingleFileUpload</h5>
<span class='badge badge-success'>06.10.2026 8:13:57 PM</span>
<span class='badge badge-danger'>06.10.2026 8:13:57 PM</span>
<span class='badge badge-default'>00:00:00:190</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=32</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:13:57 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
        <li class="test-item"  status="pass" test-id="33"
          author=""
          tag=""
          device="">
          <div class="test-detail">
            <p class="name">verifyMultipleFileUpload</p>
            <p class="text-sm">
              <span>8:14:02 PM</span> / <span>00:00:00:162</span>
              <span class="badge pass-bg log float-right">Pass</span>
            </p>
          </div>
          <div class="test-contents d-none">
<div class="detail-head">
<div class="p-v-10">
<div class="info">
<h5 class="test-status text-pass">verifyMultipleFileUpload</h5>
<span class='badge badge-success'>06.10.2026 8:14:02 PM</span>
<span class='badge badge-danger'>06.10.2026 8:14:02 PM</span>
<span class='badge badge-default'>00:00:00:162</span>
&middot; <span class='uri-anchor badge badge-default'>#test-id=33</span>
<span title='Skip to the next failed step' class='badge badge-danger pointer float-right ne ml-1'><i class="fa fa-fast-forward"></i></span>
<span title='Collapse all nodes' class='badge badge-default pointer float-right ct ml-1'><i class="fa fa-compress"></i></span>
<span title='Expand all nodes' class='badge badge-default pointer float-right et'><i class="fa fa-expand"></i></span>
</div>
</div>
</div><div class="detail-body mt-4">
<table class="table table-sm">
  <thead><tr><th class="status-col">Status</th><th class="timestamp-col">Timestamp</th><th class="details-col">Details</th></tr></thead>
  <tbody>
      <tr class="event-row">
        <td><span class="badge log pass-bg">Pass</span></td>
        <td>8:14:02 PM</td>
        <td>
          Test Passed
        </td>
      </tr>
  </tbody>
</table>
</div>
          </div>
        </li>
      </ul>
    </div>
  </div>
<div class="test-content scrollable">
<div class="test-content-tools">
<ul><li><a class="back-to-test" href="#"><i class="fa fa-arrow-left"></i></a></li></ul>
</div>
<div class="test-content-detail"><div class="detail-body"></div></div>
</div></div>
<div class="test-wrapper row view exception-view attributes-view">
<div class="test-list">
<div class="test-list-tools">
<ul class="tools pull-left"><li><a href=""><span class="font-size-14">Exception</span></a></li></ul>
<ul class="tools text-right"><li><a href="#"><span class="badge badge-primary">1</span></a></li></ul>
</div>
<div class="test-list-wrapper scrollable">
<ul class="test-list-item">
<li class="test-item">
<div class="test-detail">
<span class="meta">
<span class='badge log badge-danger'>1</span>
</span>
<p class="name">java.lang.IndexOutOfBoundsException</p>
<p class="duration text-sm">1 tests</p>
</div>
<div class="test-contents d-none">
<div class="info">
<h4>java.lang.IndexOutOfBoundsException</h4>
<span status="fail" class='badge log badge-danger'>1 failed</span>
</div>
<table class='table table-sm mt-4'>
<thead>
<tr>
<th class="status-col">Status</th>
<th class="timestamp-col">Timestamp</th>
<th>TestName</th>
</tr>
</thead>
<tbody>
<tr class="tag-test-status" status="fail">
<td><span class="badge log fail-bg">Fail</span></td>
<td>20:09:19 PM</td>
<td>
<a href="#" class="linked" test-id='12' id='12'>testFooterLinks</a>
</td>
</tr>
</tbody>
</table>
</div>
</li>
</ul>
</div>
</div>
<div class="test-content scrollable">
<div class="test-content-detail">
<div class="detail-body"></div>
</div>
</div>
</div><div class="container-fluid p-4 view dashboard-view">
<div class="row">
<div class="col-md-3">
<div class="card"><div class="card-body">
<p class="m-b-0">Started</p>
<h3>Jun 10, 2026 08:07:26 PM</h3>
</div></div>
</div>
<div class="col-md-3">
<div class="card"><div class="card-body">
<p class="m-b-0">Ended</p>
<h3>Jun 10, 2026 08:14:03 PM</h3>
</div></div>
</div>
<div class="col-md-3">
<div class="card"><div class="card-body">
<p class="m-b-0 text-pass">Tests Passed</p>
<h3>32</h3>
</div></div>
</div>
<div class="col-md-3">
<div class="card"><div class="card-body">
<p class="m-b-0 text-fail">Tests Failed</p>
<h3>1</h3>
</div></div>
</div>
</div>
<div class="row">
<div class="col-md-6">
<div class="card">
<div class="card-header">
<h6 class="card-title">Tests</h6>
</div>
<div class="card-body">
<div class="">
<canvas id='parent-analysis' width='115' height='90'></canvas>
</div>
</div>
<div class="card-footer">
<div><small data-tooltip='96%'>
<b>32</b> tests passed
</small>
</div>
<div>
<small data-tooltip='3%'><b>1</b> tests failed,
<b>0</b> skipped, <b data-tooltip='0%'>0</b> others
</small>
</div>
</div>
</div>
</div>
<div class="col-md-6">
<div class="card">
<div class="card-header">
<h6 class="card-title">Log events</h6>
</div>
<div class="card-body">
<div class="">
<canvas id='events-analysis' width='115' height='90'></canvas>
</div>
</div>
<div class="card-footer">
<div><small data-tooltip='96%'><b>32</b> events passed</small></div>
<div>
<small data-tooltip='3%'><b>1</b> events failed,
<b data-tooltip='%'>0</b> others
</small>
</div>
</div>
</div>
</div>
</div>
<div class="row"><div class="col-md-12">
<div class="card"><div class="card-header"><p>Timeline</p></div>
<div class="card-body pt-0"><div>
<canvas id="timeline" height="120"></canvas>
</div></div>
</div>
</div></div>
<script>
var timeline = {
"verifySimpleAlert":0.135,"verifyConfirmationAccept":0.137,"verifyConfirmationDismiss":0.135,"verifyPromptAlert":0.141,"verifyPopupWindow":1.964,"testAllDatePickers":0.71,"testDoubleClickCopyText":0.241,"automateDownloadFiles":16.857,"testDragAndDrop":0.333,"verifyDropDown":23.729,"verifyStartStopStartButton":4.276,"testFooterLinks":20.703,"testForm":6.723,"automateHiddenAjax":8.666,"verifyLabelsAndLinks":83.429,"verifyMouseHover1":0.397,"verifyMouseHover2":0.38,"verifyHomeNavigation":5.347,"verifyUdemyCoursesNavigation":7.849,"verifyOnlineTrainingsNavigation":5.948,"verifyBlogNavigation":4.95,"verifyPlaywrightPracticeNavigation":5.181,"verifyPaginationWebTable":10.883,"verifyShadowDomElements":0.422,"verifySliderMovement":2.425,"verifySVGElements":3.073,"verifyCellData":0.027,"verifyColumnCount":0.016,"verifyRowCount":0.016,"verifySearchInTable":0.046,"verifyWikipediaSearch":3.205,"verifySingleFileUpload":0.19,"verifyMultipleFileUpload":0.162
};
</script>
<div class="row">
<div class="col-lg-6 col-md-12 sysenv-container">
<div class="card">
<div class="card-header"><p>System/Environment</p></div>
<div class="card-body pb-0 pt-0"><table class="table table-sm table-bordered">
<thead><tr class="bg-gray"><th>Name</th><th>Value</th></tr></thead>
<tbody>
<tr>
<td>Project</td>
<td>TestAutomationHybridFramework</td>
</tr>
<tr>
<td>Tester</td>
<td>Shaurya Chattopadhyay</td>
</tr>
<tr>
<td>Environment</td>
<td>QA</td>
</tr>
<tr>
<td>Browser</td>
<td>chrome</td>
</tr>
<tr>
<td>OS</td>
<td>Windows 11</td>
</tr>
<tr>
<td>Java Version</td>
<td>17.0.18</td>
</tr>
</tbody>
</table></div>
</div>
</div>
</div>
</div>
<script>
var statusGroup = {
parentCount: 5,
passParent: 32,
failParent: 1,
warningParent: 0,
skipParent: 0,
childCount: 5,
passChild: 0,
failChild: 0,
warningChild: 0,
skipChild: 0,
infoChild: 0,
grandChildCount: 5,
passGrandChild: 0,
failGrandChild: 0,
warningGrandChild: 0,
skipGrandChild: 0,
infoGrandChild: 0,
eventsCount: 5,
passEvents: 32,
failEvents: 1,
warningEvents: 0,
skipEvents: 0,
infoEvents: 0
};
</script>        </div>
      </div>
    </div>
  </div>
<script src="https://cdn.jsdelivr.net/gh/extent-framework/extent-github-cdn@c05cd28cde1617b9d0c05a831daff6cb97fd9fd5/spark/js/spark-script.js"></script>
<script type="text/javascript"></script></body>
</html>
