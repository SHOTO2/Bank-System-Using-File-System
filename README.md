# Client Management System (C++ Project)

This project implements a client management system using C++. It provides functionalities to manage client data, including adding, updating, deleting, and performing transactions such as deposits and withdrawals. Below is a detailed overview of the code structure and functionalities.

## Table of Contents
- [Features](#features)
- [Code Overview](#code-overview)
- [File Structure](#file-structure)
- [How to Run](#how-to-run)
- [Usage](#usage)
- [Dependencies](#dependencies)

---

## Features
1. **Client Management**:
   - Add new clients.
   - Update client information.
   - Delete client records.
   - Search for clients by account number.

2. **Transaction Management**:
   - Deposit funds into client accounts.
   - Withdraw funds from client accounts.
   - View total balances across all clients.

3. **Data Persistence**:
   - Client information is saved in a text file (`Clients.txt`).
   - Supports reading and writing to the file.

4. **User Interface**:
   - Console-based menu system for easy navigation.

---

## Code Overview
### Main Components
1. **Structures**:
   - `sClient`: Represents a client's data, including account number, PIN code, name, phone, balance, and a flag for deletion.

2. **Utility Functions**:
   - `SplitString`: Splits a string into a vector based on a delimiter.
   - `ConvertLinetoRecord` and `ConvertRecordToLine`: Convert between file line format and `sClient` structure.

3. **File Operations**:
   - `LoadCleintsDataFromFile`: Loads client data from `Clients.txt`.
   - `SaveCleintsDataToFile`: Saves client data to `Clients.txt`.
   - `AddDataLineToFile`: Appends a new client record to the file.

4. **Client Management Functions**:
   - `ReadNewClient`: Reads new client information from the user.
   - `AddNewClient` and `AddNewClients`: Add one or more clients.
   - `DeleteClientByAccountNumber`: Marks a client for deletion and removes them from the file.
   - `UpdateClientByAccountNumber`: Updates client information.

5. **Transaction Functions**:
   - `DepositBalanceToClientByAccountNumber`: Deposits a specified amount into a client's account.
   - `ShowTotalBalances`: Displays total balances for all clients.

6. **User Interface**:
   - `ShowMainMenue`: Displays the main menu and handles user navigation.
   - `ShowTransactionsMenue`: Displays the transactions menu.

---

## File Structure
- **Source Code**: The main code is contained in a single `.cpp` file.
- **Clients.txt**: Text file used for storing client records in the following format:
