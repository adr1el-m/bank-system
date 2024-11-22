# ATM Transaction Case Study

This project is our case study for the final period of **COMPROG2 – Computer Programming 2 (JAVA)** at the University of Makati. The project simulates an **ATM Transaction System** for the **Richard Gwapo Banking Corporation (RGBC)**, with functionalities for customer and administrator operations.

## Features

### Customer Operations
1. **Start Transaction**  
   - Enter a PIN to log in (3 attempts allowed).  
   - Lock account after exceeding login attempts.
   - After successful login, access the following operations:
     - **Balance Inquiry**: View current account balance.
     - **Withdrawal**:
       - Minimum withdrawal: ₱100.
       - Denomination validation (e.g., ₱100, ₱200, etc.).
       - Ensures sufficient account balance.
     - **Deposit**:
       - Minimum deposit: ₱100.
     - **Fund Transfer**:
       - Minimum transfer: ₱1,000.
       - Includes a ₱25 service fee.
       - Validates target account and sufficient funds.
     - **Cancel**: Return to the main menu.

2. **Quit**  
   - Exit the program.

---

### Administrator Operations
Accessed via a dedicated PIN (`0000`).

1. **View All Customer Information**  
   - Displays account details for all customers, including status (Active/Locked).

2. **Add New Customer**  
   - Register new accounts with details: account number (5 digits), name, balance, PIN (4 digits), and status.

3. **Edit Customer Information**  
   - Modify customer names and account status (Active/Locked).

4. **Change Customer PIN**  
   - Update existing PIN numbers for accounts.

5. **Exit**  
   - Return to the main menu.

---

### Account Table (Sample Data)
The account table is implemented using a 2D array. Below is the initial data used:

| Account Number   | Account Name         | Balance   | PIN   | Status   |
|------------------|----------------------|-----------|-------|----------|
| 12345            | Roel Richard         | ₱5000.00  | 1111  | Active   |
| 23456            | Dorie Marie          | ₱0.00     | 2222  | Active   |
| 34567            | Railee Darrel        | ₱10000.00 | 3333  | Active   |
| 45678            | Railynne Dessirei    | ₱2500.00  | 4444  | Active   |
| 56789            | Raine Dessirei       | ₱10000.00 | 5555  | Locked   |
| 0000             | Administrator        | ₱0.00     | 0000  | Active   |

---

## Key Functionalities and Behaviors
1. **Login System**:
   - Users must provide both account number and PIN for authentication.
   - Locked accounts are restricted from logging in.
   - Administrator PIN allows access to privileged operations.

2. **Error Handling**:
   - Invalid inputs prompt user-friendly error messages.
   - Account locking prevents brute-force attacks.

3. **Transaction Logic**:
   - Withdrawal and fund transfer ensure sufficient balance.
   - Deposit and fund transfer validate minimum amounts.

4. **Dynamic Account Management**:
   - Add, edit, or update accounts during runtime.

---

## Project Requirements
1. **Array Implementation**  
   - Store account details in a 2D array.
   - Dynamically update the array during operations.

2. **Pin Validation**  
   - Ensure secure PIN-based access with account status validation.

3. **Customer Transactions**  
   - Enable balance inquiry, withdrawal, deposit, and fund transfer functions.

4. **Administrator Functions**  
   - Full account management capabilities.

---

## Submission Guidelines
1. **Video Demonstration**  
   - A recorded explanation of the case study with all members participating.

2. **Source Code**  
   - Submit the `.java` file via the provided Google Drive link.

3. **Deadline**  
   - **December 31, 2021**

---

## Notes
- Follow proper coding practices for error handling and validation.
- Ensure all operations are intuitive and user-friendly.
- GUI-based input and output are handled using `javax.swing.JOptionPane`.
