# Bug Report: BUG_ATM_001

### **Summary**
ATM allows cash withdrawal of Rs. 499, which is below the minimum withdrawal limit of Rs. 500.

### **Environment**
* **Component:** ATM Cash Dispenser Module
* **Environment:** Staging / UAT

### **Steps to Reproduce**
1. Insert ATM card and enter the correct PIN.
2. Select the **Cash Withdrawal** option.
3. Enter the withdrawal amount as **Rs. 499**.
4. Confirm the transaction.

### **Expected Result**
The ATM should reject the transaction and display an error message: *"Minimum withdrawal amount is Rs. 500."* No cash should be dispensed.

### **Actual Result**
The ATM dispenses Rs. 499 successfully, and the amount is deducted from the customer's account.

### **Severity & Priority**
* **Severity:** High (Business rule violation)
* **Priority:** High (Core functionality issue affecting users)
