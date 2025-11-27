# Fast University Flex Management System

## Overview
This is a console-based C++ application for managing university records, including admin, student, and teacher modules. It handles user authentication, record management, attendance, marks, grades, and timetables using file-based storage.

Developed as an OOP project by:  
- Saad Sohail (24K-2058)  
  
Date: Nov 27, 2025  

For more details, refer to the [Project Report](OOP-ProjectReport.docx).

## Requirements
- **Operating System**: Windows (due to `system("cls")` and `system("color CF")` commands).  
- **Compiler**: Any C++ compiler (e.g., g++, MinGW, Visual Studio).  
- **Libraries**: Standard C++ libraries only (no external dependencies).  

## Setup
1. **Clone the Repository**  
   ```
   git clone https://github.com/yourusername/fast-university-flex.git
   cd fast-university-flex
   ```

2. **Create Required Text Files**  
   In the project root folder, create these empty files (used for data storage):  
   - `admin.txt`  
   - `Teacher.txt`  
   - `Student.txt`  

3. **Initialize Admin Credentials**  
   Open `admin.txt` and add the following line (username: Alamraza, password: 1234):  
   ```
   Alamraza 1234
   ```

## How to Compile and Run
1. **Compile the Code**  
   Using g++ (e.g., via MinGW or command prompt):  
   ```
   g++ main.cpp -o fastuni.exe
   ```  
   Or use an IDE like Dev-C++, Code::Blocks, or Visual Studio:  
   - Open `main.cpp`.  
   - Build and run.  

2. **Run the Executable**  
   ```
   fastuni.exe
   ```  
   (Or run from your IDE.)  

   The console will display the main menu:  
   ```
   >>>>>>> Fast University Flex <<<<<<

   ------------------------------------
   |0. Exit                          |
   |1. Administrator Module          |
   |2. Student Module                |
   |3. Teacher Module                |
   ------------------------------------
   Select option:
   ```

## Default Credentials for Testing
- **Admin**:  
  Username: `saadsohail`  
  Password: `1234`  

- **Student** (Hardcoded for demo):  
  Username: `Haji`  
  Password: `123`  

- **Teachers/Students**: Add new ones via the Admin module. Generated IDs are department-based (e.g., CS-1).  

## Usage Guide
- **Admin Module**: Add/edit/view teachers and students, generate IDs.  
- **Student Module**: View attendance, marks, grades, courses, fee status.  
- **Teacher Module**: View timetable, mark attendance, assign marks/grades.  

Press Enter or follow prompts after actions. Use `system("pause")` to pause screens.

## Notes
- This is a console app – no GUI.  
- Data persists in text files (comma-separated).  
- For production, consider adding better security (e.g., hashed passwords) and dynamic storage.  
- If issues: Ensure files are in the same directory as the executable.  

## Troubleshooting
- **Compilation Errors**: Check C++11+ support.  
- **File Not Found**: Verify text files exist and are writable.  
- **Input Issues**: Enter valid data to avoid crashes (code has basic validation).  

For questions, open an issue on GitHub!
