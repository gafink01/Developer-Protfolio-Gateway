# 💻 Project Portfolio Gateway

**Author:** Garrett Finke  
**Course:** CIS352 – Intro to Enterprise Computing  

---

## 👋 About This Repository

Welcome to my GitHub portfolio repository!  
This repository serves as a central hub for showcasing my coursework and technical projects. Each project demonstrates key enterprise computing concepts using COBOL and related technologies.

---

## 👤 About the Author

### Garrett Finke

I am currently studying Networking at Wayne State College.  
I am going to be a senior and am currently on the college's Esports Valorant team.  
I have experience with programming languages such as Java, C++, and Python.

- GitHub: https://github.com/gafink01  
- Email: gafink01@wsc.edu  

---

## 📚 Table of Contents

## 📚 Table of Contents

| Project | Tech | Category | Description | Authors | Repo |
|--------|------|----------|-------------|---------|------|
| [CALC2000](#calc2000) | COBOL | CIS352 | Calculates future investment values using compound interest and doubling logic | Garrett Finke, Grant Peverett | [Repo Link](#) |
| [UTIL2000](#util2000) | COBOL | CIS352 | Calculates electric utility bills using a tiered kWh rate system | Garrett Finke | [Repo Link](#) |

## CALC2000

CALC2000 is a COBOL program that calculates the future value of an investment over a number of years using a set interest rate.  
The program runs multiple scenarios by doubling the investment amount each time, demonstrating iterative processing and financial calculations.
Collaberators include Garrett Finke, and Grant Peverett.

**Key Concepts:**  
COMPUTE statements | PERFORM loops | Iteration | Numeric calculations | ROUNDED option  

**Tech Stack:**
- COBOL  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Example Output
## CALC2000

CALC2000 is a COBOL program that calculates the future value of an investment over a fixed number of years using a set interest rate.  
The program works by doubling the investment amount each time, demonstrating the processes of the financial calculations.

**Key Concepts:**  
COMPUTE statements | PERFORM loops | Iteration | Numeric calculations | ROUNDED option  

**Tech Stack:**
- COBOL  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Example Output

```
***************************************
*        CALC2000 Investment Tool      *
***************************************

Calculating Future Values

Investment Amount :     1,000
Future Value      :     1,628.89

Investment Amount :     2,000
Future Value      :     3,257.79

Investment Amount :     4,000
Future Value      :     6,515.58

End of session.
```

🔙 [Back to TOC](#-table-of-contents)
## UTIL2000

UTIL2000 is a COBOL utility billing program that calculates electric bills for multiple customers using a set pricing system.  
It applies different rates depending on power usage and adds a fixed service fee to generate a final total bill.

**Key Concepts:**  
Tiered rate calculations | Conditional logic | Arithmetic operations | Data movement | Formatted output  

**Tech Stack:**
- COBOL  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Example Output

```
********************************
*** UTIL2000 - CUSTOMER BILL ***
********************************

--------------------------------
CUSTOMER: CUST-ALPHA
--------------------------------
KWH USED       :   350
SERVICE FEE    : $14.95
TIER 1 CHARGE  : $42.00
TIER 2 CHARGE  :  $0.00
TIER 3 CHARGE  :  $0.00
--------------------------------
TOTAL BILL     : $56.95
--------------------------------

--------------------------------
CUSTOMER: CUST-BRAVO
--------------------------------
KWH USED       :   925
SERVICE FEE    : $14.95
TIER 1 CHARGE  : $60.00
TIER 2 CHARGE  : $63.75
TIER 3 CHARGE  :  $0.00
--------------------------------
TOTAL BILL     : $138.70
--------------------------------
```

🔙 [Back to TOC](#-table-of-contents)
## RPT2000

RPT2000 is a COBOL Year-To-Date (YTD) sales reporting program that reads customer master records from a file and generates a formatted report.  
It calculates year-over-year performance, including change amounts and percentage differences, and produces grand totals for all qualifying customers.

This program demonstrates real enterprise-style reporting using file processing, control logic, and formatted output.

**Key Concepts:**  
Sequential file processing | Report generation | COMPUTE calculations | Percentage change | Pagination | Grand totals  

**Tech Stack:**
- COBOL  
- JCL (mainframe-style execution)  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Example Output

```
DATE:  02/19/2026           YEAR-TO-DATE SALES REPORT            PAGE:    1
TIME:  14:35                                                      RPT2001

BRANCH SALES  CUST   CUSTOMER NAME         SALES          SALES        CHANGE    CHANGE
 NUM    REP   NUM                         THIS YTD       LAST YTD      AMOUNT   PERCENT
------  -----  -----  --------------------  ----------  ----------  ----------  ------
 01      10   10001  ACME SUPPLY CO          25,450.75   20,125.50    5,325.25    26.5
 02      08   20002  SOUTHERN MATERIALS      45,300.25   30,100.00   15,200.25    50.5

                                           ===========  ===========  ===========  ======
                              GRAND TOTAL   89,651.00    69,725.50   19,925.50    28.6
```

🔙 [Back to TOC](#-table-of-contents)
