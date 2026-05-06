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

| Project | Tech | Category | Description | Repo |
|--------|------|----------|-------------|------|
| [CALC2000](#calc2000) | COBOL | CIS352 | Calculates future investment values using compound interest and doubling logic | [Repo Link](#) |
| [UTIL2000](#util2000) | COBOL | CIS352 | Calculates electric utility bills using tiered kWh rate system | [Repo Link](#) |

---

## CALC2000

A foundational COBOL program that calculates the future value of an investment using a fixed interest rate over a set number of years. The program runs three iterations, doubling the investment amount each time.

**Key Concepts:**  
COMPUTE statements | PERFORM loops | Numeric calculations | ROUNDED option  

**Tech Stack:**
- COBOL  
- VS Code  
- GitHub  

### 🚦 Status
✅ Completed  

### 📄 Source Code

```cobol
       IDENTIFICATION DIVISION.
       PROGRAM-ID. CALC2000.
       DATA DIVISION.
       WORKING-STORAGE SECTION.

       01 INVESTMENT-AMOUNT     PIC 9(5)   VALUE 1000.
       01 NUMBER-OF-YEARS       PIC 99     VALUE 10.
       01 YEARLY-INTEREST-RATE  PIC 99V9   VALUE 5.5.

       01 FUTURE-VALUE          PIC 9(7)V99 VALUE 0.
       01 YEAR-COUNTER          PIC 999     VALUE 0.

       PROCEDURE DIVISION.

       PERFORM CALC-ROUTINE 3 TIMES.
       DISPLAY "End of session."
       STOP RUN.

       CALC-ROUTINE.
           MOVE INVESTMENT-AMOUNT TO FUTURE-VALUE
           MOVE 1 TO YEAR-COUNTER

           PERFORM UNTIL YEAR-COUNTER > NUMBER-OF-YEARS
              COMPUTE FUTURE-VALUE =
                 FUTURE-VALUE + (FUTURE-VALUE * YEARLY-INTEREST-RATE / 100)
              ADD 1 TO YEAR-COUNTER
           END-PERFORM

           DISPLAY "Investment: " INVESTMENT-AMOUNT
           DISPLAY "Future Value: " FUTURE-VALUE

           COMPUTE INVESTMENT-AMOUNT = INVESTMENT-AMOUNT * 2.
