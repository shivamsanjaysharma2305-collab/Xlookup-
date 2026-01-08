# Xlookup-
shivamssharma86@gmail.com

✅ 1. Basic Search – Lookup Department

Goal: Fetch the Department for each EmpID in Performance_Review.

Formula (Department column):

=XLOOKUP(B2, Employee_Master!A:A, Employee_Master!D:D)

✅ 2. Spill Array – Return First & Last Name Together

Goal: Return First Name and Last Name for EmpID E004 using one formula.

Formula (e.g., cell A10):

=XLOOKUP("E004", Employee_Master!A:A, Employee_Master!B:C)


📌 This spills into two cells automatically.

✅ 3. Error Handling – Annual Salary Lookup

Goal: Populate Annual Salary and show "Contractor" if EmpID is missing (E999).

Formula (Annual Salary column):

=XLOOKUP(B2, Employee_Master!A:A, Employee_Master!E:E, "Contractor")

✅ 4. Calculation – Computed Bonus

Goal: Calculate bonus using salary lookup × bonus multiplier.

Formula (Computed Bonus column):

=XLOOKUP(B2, Employee_Master!A:A, Employee_Master!E:E, 0) * F2


📌 Handles missing employees by returning 0 instead of an error.

✅ 5. Left Lookup – Find EmpID Using Last Name

Goal: Find EmpID for last name "Kent"
(This cannot be done using VLOOKUP)

Formula:

=XLOOKUP("Kent", Employee_Master!C:C, Employee_Master!A:A)

✅ 6. Missing Data Check – Employees Not Reviewed

Goal: Identify EmpIDs in Employee_Master missing from Performance_Review.

Formula (helper column):

=XLOOKUP(A2, Performance_Review!B:B, Performance_Review!B:B, "Not Reviewed")


📌 Employees returning "Not Reviewed" do not appear in Performance_Review.

🚀 Key Skills Demonstrated

✔ XLOOKUP (basic & advanced)

✔ Spill arrays

✔ Error handling with if_not_found

✔ Left lookups

✔ Dynamic calculations

✔ Data validation across worksheets

🛠 Tools Used

Microsoft Excel (Office 365 / Excel 2021+)

XLOOKUP Function

📎 Conclusion

This project showcases how XLOOKUP replaces VLOOKUP, HLOOKUP, INDEX & MATCH with cleaner, more powerful formulas suitable for HR, Finance, and Analytics roles.
