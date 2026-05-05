# IT3040_Assignment1_IT23816954
Transliteration Testing using Playwright
# IT3040 – ITPM Assignment 1

## Transliteration Accuracy Testing (Singlish to Sinhala)

---

## Student Information

Name: Athapaththu I N
Registration Number: IT23816954
Module: IT3040 – ITPM
Assignment: Assignment 1 – Option 1

---

## Project Overview

This project evaluates the accuracy of a chat-style Singlish to Sinhala transliteration system available at:
https://www.pixelssuite.com/chat-translator

The objective is to identify scenarios where the system fails to correctly convert Singlish inputs into Sinhala outputs. A total of 50 negative test cases were designed and automated using Playwright.

---

## Objectives

* Test the transliteration accuracy of the system
* Identify incorrect or inconsistent outputs
* Cover all 24 Singlish input types
* Automate test execution using Playwright
* Record results in a structured Excel sheet

---

## Technologies Used

* Python
* Playwright
* openpyxl
* Visual Studio Code

---

## Project Structure

project-folder/
│
├── test_automation.py
├── Assignment 1 - Test cases.xlsx
├── README.md
 

---

## Setup Instructions

### 1. Install Python

Install Python (version 3.8 or above)

### 2. Install Required Packages

pip install playwright openpyxl
playwright install

### 3. Run the Automation Script

py test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open

---

## Test Case Details

Total Test Cases: 50 (Negative Test Cases)
Test Case ID Format: Neg_0001 – Neg_0050
Input Types Covered: All 24 categories (minimum 2 each)

Each test case includes:

* Actual Output
* Status (Pass/Fail)
* Singlish Input Types Covered
* Evidence or rationale

---

## Files Included

* Playwright automation script
* Completed Excel file
* README documentation

---

## Notes

This testing focuses only on chat-style transliteration accuracy. Backend, performance, and security testing are not included.

Some failures may occur due to:

* Incorrect Sinhala word generation
* Output not updating correctly
* System errors such as "Failed to fetch"

---

## Repository Access

This repository is publicly accessible as required for evaluation.

---

## Conclusion

The system demonstrates several inconsistencies when handling informal Singlish inputs, particularly in cases involving slang, mixed-language content, and spelling variations. This highlights the need for improved handling of real-world user inputs in transliteration systems.

---
