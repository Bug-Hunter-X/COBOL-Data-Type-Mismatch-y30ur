# COBOL Data Type Mismatch Bug

This repository demonstrates a common error in COBOL programming: using an alphanumeric field where a numeric field is required. The code has a data type mismatch where `WS-AREA-2` is defined as a numeric field but is treated as an alphanumeric field within the MOVE statement, causing unexpected output.

## Bug Description

The program attempts to display an alphanumeric string (`WS-AREA-1`) and a numeric value (`WS-AREA-2`). However, if the value in `WS-AREA-2` is used in further arithmetic operations, it will lead to incorrect results.

## Solution

To correct the bug, ensure the data types are correctly aligned with their intended use.  The `bugSolution.cob` file demonstrates the fix.