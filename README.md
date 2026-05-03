 # Hybrid Inventory Manager (Capstone Project)

## 📌 Project Overview

This project is a **Hybrid Inventory Manager** where:

* The **backend is written in C** using structs and binary file storage
* The **frontend is written in C++** using classes and STL

The application allows users to manage inventory items using a console-based menu.

---

## ⚙️ Features

* Add new item (unique ID required)
* View item by ID
* Update existing item
* Delete item (soft delete)
* List all items
* Data persistence using binary file (`inventory.dat`)

---

## 🧱 Technologies Used

* C (for file handling and data storage)
* C++ (for UI and logic)
* STL (`vector`, `sort`)
* Binary file handling (`fread`, `fwrite`, `fseek`)

---

## 📂 Project Structure

```
inventory_project/
├── include/
│   └── inventory.h
├── src/
│   ├── inventory.c
│   ├── InventoryManager.cpp
│   └── main.cpp
├── Makefile
├── inventory.dat (auto-created)
└── README.md
```

---

## 🛠️ Build Instructions (Windows - MinGW)

### Compile:

```
g++ src/main.cpp src/InventoryManager.cpp src/inventory.c -o app.exe
```

### Run:

```
.\app.exe
```

---

## 🧪 Test Cases

* Add 3 items, exit program, run again → items should still exist
* Update an item → changes should persist after restart
* Delete an item → it should not appear in list/view
* Try adding duplicate ID → should be rejected
* View item with invalid ID → should show "Not found"

---

## 🧠 Key Concepts Used

* **Structs in C** for data representation
* **Binary file storage** for persistence
* **fread / fwrite / fseek** for file operations
* **Soft delete** using `is_deleted` flag
* **C and C++ integration** using `extern "C"`
* **STL vector and sort** for managing and displaying data

---

## 🎯 Conclusion

This project demonstrates how C and C++ can be combined to build a hybrid system where:

* C handles low-level data storage
* C++ manages user interaction and higher-level logic

---

## 👤 Author

Name: Kirti Tamboli
Roll No: 1214
