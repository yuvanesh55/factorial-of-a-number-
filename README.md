# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
 MOV DPTR,#4500H 
 MOVX A,@DPTR 
 MOV R0,A 
 INC DPTR 
 ACALL FACTORIAL 
 MOVX @DPTR,A 
 SJMP THIN 

FACTORIAL: DEC R0
 CJNE R0,#01H,PRODUCT
 SJMP THICK 

PRODUCT: MOV B,R0 
 MUL AB
 ACALL FACTORIAL 

THICK: RET 
THIN: RET 
END

```
OUTPUT

<img width="760" height="320" alt="WhatsApp Image 2026-05-12 at 11 42 55 AM" src="https://github.com/user-attachments/assets/3dc44bd9-5a79-464f-b79e-a57dbb5bb2ae" />


---
MANUAL CALCULATIONS

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/4d9b10f5-b010-4418-af80-488d92eb0acf" />


---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---



1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END

```
OUTPUT

(Keil output screenshot can be inserted here)

---
MANUAL CALCULATIONS

---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


