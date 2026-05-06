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
I am a senior and currently on the college's Esports Valorant team.  
I have experience with programming languages such as Java, C++, and Python.

- GitHub: https://github.com/gafink01  
- Email: gafink01@wsc.edu  

---

## 📚 Table of Contents

| Project | Tech | Category | Description | Authors | Repo |
|--------|------|----------|-------------|---------|------|
| [CALC2000](#calc2000) | COBOL | CIS352 | Calculates future investment values using compound interest and doubling logic | Garrett Finke, Grant Peverett | [CALC2000](https://github.com/gafink01/Cobol-CALC2000) |
| [UTIL2000](#util2000) | COBOL | CIS352 | Calculates electric utility bills using a tiered kWh rate system | Garrett Finke | [UTIL2000](https://github.com/gafink01/UTIL2000) |
| [RPT2000](#rpt2000) | COBOL | CIS352 | Generates a YTD sales report with year-over-year comparisons and grand totals | Garrett Finke | [RPT2000](https://github.com/gafink01/RPT200) |
| [RPT5000](#rpt5000) | COBOL | CIS352 | Three-level YTD sales report with sales rep and branch control breaks using an EVALUATE | Garrett Finke & Gabriel Dilley | [RPT5000](https://github.com/gawdilley/COBOL-Chapter-5-Assignment) |

---

## CALC2000

CALC2000 is a COBOL program that calculates the future value of an investment over a fixed number of years using a set interest rate.  
The program runs multiple scenarios by doubling the investment amount each time, demonstrating iterative processing and financial calculations.

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

Investment Amount :     2,500
Future Value      :     4,064.74

Investment Amount :     5,000
Future Value      :     8,129.49

Investment Amount :    10,000
Future Value      :    16,258.98

End of session.
```

🔙 [Back to TOC](#-table-of-contents)

---

## UTIL2000

UTIL2000 is a COBOL utility billing program that calculates electric bills for multiple customers using a tiered pricing system.  
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
KWH USED       :   610
SERVICE FEE    : $16.25
TIER 1 CHARGE  : $60.00
TIER 2 CHARGE  : $16.50
TIER 3 CHARGE  : $0.00
--------------------------------
TOTAL BILL     : $92.75
--------------------------------

--------------------------------
CUSTOMER: CUST-BRAVO
--------------------------------
KWH USED       :   980
SERVICE FEE    : $16.25
TIER 1 CHARGE  : $60.00
TIER 2 CHARGE  : $72.00
TIER 3 CHARGE  : $0.00
--------------------------------
TOTAL BILL     : $148.25
--------------------------------

--------------------------------
CUSTOMER: CUST-CHARLIE
--------------------------------
KWH USED       :  1450
SERVICE FEE    : $16.25
TIER 1 CHARGE  : $60.00
TIER 2 CHARGE  : $75.00
TIER 3 CHARGE  : $81.00
--------------------------------
TOTAL BILL     : $232.25
--------------------------------
```

🔙 [Back to TOC](#-table-of-contents)

---

## RPT2000

RPT2000 is a COBOL Year-To-Date (YTD) sales reporting program that reads customer master records from a file and generates a formatted report.  
It calculates year-over-year performance, including change amounts and percentage differences, and produces grand totals for all qualifying customers.

This program demonstrates enterprise-style report generation using file processing, control breaks, calculations, and formatted output.

**Key Concepts:**  
Sequential file processing | Report generation | COMPUTE calculations | Percentage change | Control breaks | Grand totals  

**Tech Stack:**
- COBOL  
- JCL (mainframe-style execution)  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Example Output

```
DATE:  02/19/2026           YEAR-TO-DATE SALES REPORT                     PAGE:    1
TIME:  14:35                                                                 RPT2001

BRANCH SALES  CUST         CUSTOMER NAME       SALES       SALES      CHANGE  CHANGE
NUM    REP    NUM   --------------------  ----------  ----------  ----------  ------
03     11     11012  WESTLAKE INDUSTRIES   38,600.40   29,450.10    9,150.30    31.1
04     07     22045  NORTHRIDGE SUPPLY     52,980.75   41,120.50   11,860.25    28.8

                            GRAND TOTAL   91,581.15    70,570.60   21,010.55    29.8
```

🔙 [Back to TOC](#-table-of-contents)

## RPT5000

RPT5000 is an enterprise COBOL Year-To-Date sales reporting program that reads customer master records and produces a formatted report using control breaks.

It calculates customer-level sales changes, salesrep totals, branch totals, grand totals, and percent change with divide-by-zero protection. The program demonstrates advanced sequential file processing and hierarchical report generation.

**Key Concepts:** Sequential file processing | Control breaks | Nested totals | COMPUTE statements | Report formatting | Percent calculations | EOF handling  

### 🚦 Status
✅ Completed  

### Example Output

DATE: 03/26/2026        YEAR-TO-DATE SALES REPORT        PAGE: 1
TIME: 14:35                                            RPT5000

BRANCH  SLSREP  CUST   CUSTOMER NAME         SALES THIS YTD   SALES LAST YTD   CHANGE   %
-----------------------------------------------------------------------------------------
03      11      11012  WESTLAKE INDUSTRIES    38,600.40        29,450.10        9,150.30  31.1
03      11      11013  RIVER TECH             44,120.75        39,500.25        4,620.50  11.7

                    SALESREP TOTAL            82,721.15        68,950.35       13,770.80  20.0
                    BRANCH TOTAL              82,721.15        68,950.35       13,770.80  20.0

GRAND TOTAL                                  82,721.15        68,950.35       13,770.80  20.0
GRAND TOTAL    99,201.45 84,310.95 14,890.50 17.6
```

🔙 [Back to TOC](#-table-of-contents)
