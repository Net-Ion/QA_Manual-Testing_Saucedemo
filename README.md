# QA_Manual-Testing_Saucedemo
SauceDemo QA Testing Project

About the Project

This is a manual QA testing project for SauceDemo, a sample e-commerce web application provided by Sauce Labs.

I created this project to practice the software testing process from writing test cases and executing them to identifying and documenting defects.

The project focuses on four main modules:

Login

Inventory / Products

Your Cart

Checkout

Application: SauceDemo
URL: https://www.saucedemo.com/
Testing Type: Manual Functional Black-Box Testing
Browser: Google Chrome
Test User: standard_user

Project Objective

The objective of this project is to verify the main e-commerce workflows and identify issues through structured manual testing.

The testing process followed in this project is:

Understand Requirements
        ↓
Create Test Scenarios
        ↓
Write Test Cases
        ↓
Execute Test Cases
        ↓
Record PASS / FAIL
        ↓
Report Defects
        ↓
Maintain RTM
        ↓
Prepare Test Summary

Modules Tested

Login

Valid credentials

Invalid username

Invalid password

Empty username

Empty password

Empty username and password

Login error messages

Inventory

Product listing

Product names

Product prices

Product sorting

Product details

Add to cart

Remove from cart

Sorting dropdown functionality

Your Cart

Opening the cart

Product visibility

Multiple products

Cart item count

Removing products

Continue Shopping

Checkout navigation

Empty-cart behavior

Checkout

Customer information

Required fields

Postal code validation

Checkout overview

Order completion

Cancel/navigation behavior

Test Results

A total of 35 test cases were included in the test suite.

Module

Test Cases

Passed

Failed

Login

6

6

0

Inventory

11

9

2

Your Cart

10

9

1

Checkout

8

7

1

Total

35

31

4

Pass Rate: 88.57%

Defects Found

Four defects were documented during testing.

Bug ID

Module

Description

Severity

Priority

Bug-01

Inventory

Incorrect product name displayed

Low

P3

Bug-02

Inventory

Sorting dropdown arrow not clickable

Low

P3

Bug-03

Your Cart

Checkout can be accessed from an empty cart without a warning message

Medium

P2

Bug-04

Checkout

Invalid postal code is accepted and Checkout Overview is displayed

High

P1

Each defect contains the related test case, preconditions, reproduction steps, expected result, actual result, severity, priority and status.

Requirement Traceability Matrix

An RTM was created to connect functional requirements with the test cases used to verify them.

Requirement
    ↓
Test Case
    ↓
Test Execution
    ↓
PASS / FAIL
    ↓
Defect (if applicable)

The RTM is available as a separate sheet in the main Excel workbook.

Test Execution

The recorded execution results are:

35 total test cases

31 passed

4 failed

4 defects reported

88.57% pass rate

The detailed execution report is available in Test_Execution_Report.docx.

Test Plan

The project includes a test plan covering:

Testing objective

Scope

Out-of-scope areas

Testing approach

Test environment

Test data

Entry criteria

Exit criteria

Deliverables

Risks and notes

File: Test_Plan.docx

Test Summary Report

The test summary report contains:

Overall test results

Pass/fail statistics

Defect summary

Key findings

QA deliverables

File: Test_Summary_Report.docx

Tools Used

Microsoft Excel — test cases, RTM, execution tracking and bug report

Microsoft Word — test plan and test summary

Google Chrome — application testing

Git / GitHub — version control and project documentation

Project Structure

SauceDemo-QA-Testing/
│
├── README.md
├── SauceDemo_QA_Testing_Final.xlsx
├── Test_Plan.docx
├── Test_Execution_Report.docx
└── Test_Summary_Report.docx

Excel Workbook Sheets

Summary
RTM
Test Execution
Login Page
Inventory
Your Cart
Checkout
Bug Report

What I Learned

Through this project, I practiced:

Understanding functional requirements

Creating test scenarios

Writing structured test cases

Positive and negative testing

Manual test execution

Identifying and documenting defects

Severity and priority

Requirement traceability

Test execution reporting

Test summary reporting

Organizing QA documentation

Future Improvements

The current project focuses on manual testing. I plan to extend it with:

JIRA for defect tracking

SQL for database validation

Postman for API testing

Basic Selenium automation

Regression test suites

Screenshots and additional execution evidence

Disclaimer

This is a personal QA practice and portfolio project based on a publicly accessible demo application.

It is not client work or production testing. The project is intended to demonstrate my understanding of manual QA testing and related documentation.
