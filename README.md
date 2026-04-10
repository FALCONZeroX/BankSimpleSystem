# 🏦 Bank Management System FP (Functional Programming) - C++

![C++](https://img.shields.io/badge/C++-Solutions-blue.svg?style=flat&logo=c%2B%2B)
![Year](https://img.shields.io/badge/Year-2026-green)
![Author](https://img.shields.io/badge/Created%20By-FALCON-orange)

A comprehensive and lightweight banking management system built with **C++**. This project focuses on managing client data and system users through a robust permissions-based architecture.

This project is a personal implementation as part of **Course 8** in the programming series by **Dr. Mohammed Abu-Hadhoud**.

---

## 🚀 Key Features

The system is divided into several modules ensuring secure and efficient management:

### 1. User Management & Permissions
* **Secure Login:** Features a login screen requiring a username and password with a maximum of 3 attempts before being blocked.
* **Granular Permissions:** Specific access can be granted for each user, including:
    * Show Clients
    * Add/Delete/Update Clients
    * Find Clients
    * Transactions
    * User Management
* **Admin Protection:** Built-in safeguards prevent the deletion or modification of the 'Admin' user or the currently logged-in user.

### 2. Client Management
* **Add New Clients:** Allows creating new records while validating that Account Numbers are unique.
* **Update & Delete:** Support for modifying client details or performing "Soft Deletes" to maintain data integrity.
* **Advanced Search:** Find clients instantly using their Account Number or Name.

### 3. Transaction Module
* **Deposit & Withdraw:** Handle financial operations with real-time balance updates.
* **Balance Validation:** Ensures clients have sufficient credit before allowing withdrawals.
* **Total Balances Report:** Generates a summarized report of all client balances in the system.

### 4. Data Persistence
* **File-Based Storage:** Automatically saves and loads data from text files (`.txt`), ensuring data is preserved after the program closes.

---

## ⚠️ Important Setup Instructions (Prerequisites)

To ensure the program runs successfully without errors, please follow these steps:

1.  **Mandatory Files:** You must download or create the following files:
    * `Clients.txt`
    * `Users.txt`
2.  **File Path:** These files **MUST** be placed in the same directory as the project source code or the executable file. 
3.  **Automatic Loading:** The system is designed to read from these files immediately upon startup.

---

## 🛠 Technical Stack & Concepts

* **Vectors & Structs:** Used for dynamic data management in memory.
* **File Handling (fstream):** For persistent data storage and retrieval.
* **Enums:** To manage application states, read modes, and navigation.
* **Header ASCII Art:** Custom-designed "FALCON" branding in the source code.

---

## ⚠️ Current Limitations

While the system is functional for educational purposes, it currently has the following limitations:

* **File System Dependency**: The program relies on flat `.txt` files, which may face performance issues as the data size grows significantly.
* **Concurrency**: The system does not support multiple users accessing or writing to the database files simultaneously.
* **Security**: Data in `Users.txt` and `Clients.txt` is stored in plain text, which is not suitable for real-world sensitive financial information.
* **Console-Based UI**: The interface is limited to the Windows Command Prompt, utilizing `system("cls")` and `system("color")`, which limits cross-platform compatibility.
* **No Transaction History**: While the balance updates, the system does not currently log a history of individual deposits or withdrawals.

---

## 🛠 Future Improvements (Roadmap)

To evolve this project into a more robust application, the following enhancements are planned:

* **Database Integration**: Transition from `.txt` files to a relational database like **SQLite** or **MySQL** for better data management and scalability.
* **Data Encryption**: Implement hashing algorithms (like SHA-256) for passwords and encryption for sensitive client data to enhance security.
* **Graphical User Interface (GUI)**: Develop a modern interface using frameworks like **Qt** or **SFML** to replace the current console design.
* **Transaction Logs**: Add a feature to record every transaction (Date, Time, Amount, Type) into a dedicated `Log.txt` file for auditing.
* **Networking**: Implement a Client-Server architecture to allow the system to be accessed over a local network.
* **Advanced Reports**: Add the ability to export reports in different formats like CSV or PDF for professional use.

---

## 👨‍💻 Developed By
**Falah Fathel (FALCON)**
* **Year:** 2026
* **Educational Reference:** Course 8 - Dr. Mohammed Abu-Hadhoud

---

### 📝 License
This project is intended for educational purposes and to demonstrate proficiency in C++ programming logic.
