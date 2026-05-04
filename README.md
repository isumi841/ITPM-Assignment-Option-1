# IT3040 – ITPM Assignment 1 (Option 1)

## Playwright Automation Project – Sinhala Transliteration Testing

---

## 👨‍🎓 Student Information

* **Name:** K K D I Dahamya
* **Registration Number:** IT23542938

---

## 📌 Project Overview

This project implements an automated testing solution to validate the Sinhala transliteration functionality available at:

🔗 https://www.pixelssuite.com/chat-translator

The automation script reads test cases from an Excel file, inputs Singlish text into the web application, captures the Sinhala output, compares it with expected results, and updates the Excel file with execution results automatically.

---

## 🎯 Objectives

* Automate functional testing of a Sinhala transliteration system
* Validate outputs using predefined test cases
* Reduce manual testing effort
* Improve efficiency and accuracy

---

## 🧰 Tools & Technologies

* Python
* Playwright
* openpyxl
* Microsoft Excel
* Google Chrome

---

## ⚙️ Prerequisites

Ensure the following are installed:

* Python 3.11 or 3.12
* Google Chrome (latest version)
* Stable internet connection

---

## 📦 Installation (One-Time Setup)

Run the following commands in Command Prompt:

```bash
pip install -U pip
pip install playwright openpyxl
playwright install
```

---

## 📁 Project Structure

```
IT23542938/
│── IT23542938.py
│── IT23542938.xlsx
│── IT23542938README.md
│── IT23542938.txt
```

---

## 📊 Test Data Preparation

Open the Excel file:

**IT23542938.xlsx**

Fill ONLY these columns:

* TC ID
* Input length type
* Input
* Expected output

⚠️ Do NOT fill:

* Actual output
* Status

➡️ These will be automatically updated by the script.

---

## ▶️ Run the Automation Script

Execute the following command in CMD:

```bash
py test_automation.py --excel "C:\Users\isumi\OneDrive\Desktop\IT23542938\IT23542938.xlsx" --input-col "Input" --expected-col "Expected output" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 12000 --type-delay-ms 300 --slow-mo-ms 800 --keep-open
```

---

## 📈 Output & Results

After execution:

* Excel file will be updated with:

  * **Actual output**
  * **Status (PASS / FAIL)**

### ✅ Result Meaning

* **PASS** → Actual output matches expected output
* **FAIL** → Outputs do not match

---

## 📝 Final Manual Requirement

After running the script, manually add TWO columns in Excel:

* Singlish input types covered
* Evidence / rationale for input coverage

Provide explanations based on your observations.

---

## 🚀 Features

* Automated browser interaction using Playwright
* Data-driven testing using Excel
* Automatic output validation
* Result logging into Excel
* Configurable execution parameters

---

## ⚠️ Important Notes

* Keep Excel file **closed** before running
* Do NOT rename files
* Maintain stable internet connection
* Adjust delays if needed for slower systems

---

## 🧪 Scope

* Only the Sinhala transliteration feature is tested
* Testing is based on UI behavior of the live website

---

## ✅ Conclusion

This project demonstrates how automation can be used to efficiently test a Sinhala transliteration system. It reduces manual effort, improves accuracy, and ensures consistent validation of outputs.

---
