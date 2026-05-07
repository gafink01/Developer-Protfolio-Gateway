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

<img src="GarrettImage.jpg" alt="Garrett Finke" width="200" style="border-radius: 10px;"/>

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
| [RPT6000](#rpt6000) | COBOL | CIS352 | Advanced YTD sales reporting system with multi-file processing, control breaks, salesrep lookups, and paginated enterprise reporting | Garrett Finke | [RPT6000](https://github.com/gafink01/RPT6000) | 
| [SEQ3000](#seq3000) | COBOL | CIS352 | Sequential employee master file maintenance program that processes add, change, and delete transactions while generating updated master and error files | Garrett Finke | https://github.com/gafink01/SEQ3000-ASSIGMENT.git |
---

## CALC2000

**Collaborators** 

-Garrrett Finke

-Grant Peverett

**Description**

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

**Collaborators** 

-Garrett Finke

**Description**

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

**Collaborators** 

-Garrett Finke

**Description**

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

**Collaborators** 

-Garrett Finke

**Description**

RPT5000 is an enterprise COBOL Year-To-Date sales reporting program that reads customer master records and produces a formatted report using control breaks.

It calculates customer-level sales changes, salesrep totals, branch totals, grand totals, and percent change with divide-by-zero protection. The program demonstrates advanced sequential file processing and hierarchical report generation.

**Key Concepts:** Sequential file processing | Control breaks | Nested totals | COMPUTE statements | Report formatting | Percent calculations | EOF handling  

### 🚦 Status
✅ Completed  

### Example Output

```
DATE: 03/26/2026        YEAR-TO-DATE SALES REPORT        PAGE: 1
TIME: 14:35                                            RPT5000

BRANCH  SLSREP  CUST   CUSTOMER NAME         SALES THIS YTD   SALES LAST YTD   CHANGE   %
-----------------------------------------------------------------------------------------
03      11      11012  WESTLAKE INDUSTRIES    38,600.40        29,450.10        9,150.30  31.1
03      11      11013  RIVER TECH             44,120.75        39,500.25        4,620.50  11.7

                    SALESREP TOTAL            82,721.15        68,950.35       13,770.80  20.0
                    BRANCH TOTAL              82,721.15        68,950.35       13,770.80  20.0

GRAND TOTAL                                  82,721.15        68,950.35       13,770.80  20.0
```

🔙 [Back to TOC](#-table-of-contents)

---

## RPT6000

**Collaborators**  

- Garrett Finke  

**Description**

RPT6000 is an advanced enterprise COBOL Year-To-Date (YTD) sales reporting program that reads both customer master records and sales representative files to generate a fully formatted business report using hierarchical control breaks.

The program calculates customer-level sales changes, sales representative totals, branch totals, and grand totals while also computing percentage increases and decreases with divide-by-zero protection and overflow handling. It demonstrates enterprise-style report generation through sequential file processing, indexed table lookups, multi-file integration, pagination, and formatted output commonly used in mainframe systems.

RPT6000 expands on previous reporting projects by introducing SALESREP table loading and SEARCH processing to dynamically match sales representative numbers with names during report generation.

**Key Concepts:**  
Sequential file processing | Multi-file processing | Table handling | Indexed tables | Control breaks | Nested totals | COMPUTE statements | Percentage calculations | EOF handling | Enterprise report formatting  

**Tech Stack:**  
- COBOL  
- JCL (mainframe-style execution)  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed

🔙 [Back to TOC](#-table-of-contents)

---

## SEQ3000

**Collaborators**  

- Garrett Finke  

**Description**

SEQ3000 is a COBOL sequential file maintenance program that processes employee transaction records against an existing employee master file.  
The program compares transaction and master records by employee ID and applies add, change, and delete operations to create a new updated master file while also writing invalid transactions to an error file.

The project demonstrates enterprise-style sequential file processing techniques commonly used in legacy mainframe systems. It uses multiple input/output files, file status handling, record matching logic, and transaction processing workflows.

The program currently processes records correctly in several scenarios, but it still encounters an ABEND during execution that is being debugged.

**Key Concepts:**  
Sequential file processing | File maintenance | Transaction matching | Add/change/delete logic | File status handling | EOF processing | Enterprise COBOL workflows | Error transaction reporting  

**Tech Stack:**  
- COBOL  
- VS Code  
- GitHub  
- JCL (mainframe-style execution concepts)  

### 🚦 Status
⚠️ Close to Working — Currently Debugging an ABEND Error

### 📄 Program Features

- Reads employee transactions from `EMPTRAN`
- Reads existing employee records from `OLDEMP`
- Creates updated employee master file `NEWEMP`
- Writes invalid transactions to `ERRTRAN`
- Supports:
  - Add transactions
  - Change transactions
  - Delete transactions
- Uses file status checking for error handling
- Uses HIGH-VALUES logic for EOF processing

### 📄 Example Logic Flow

```text
1. Read transaction record
2. Read old master record
3. Compare employee IDs
4. Apply transaction:
      A = Add
      C = Change
      D = Delete
5. Write updated record to NEWEMP
6. Write invalid transactions to ERRTRAN
7. Continue until EOF
```

🔙 [Back to TOC](#-table-of-contents)

---

