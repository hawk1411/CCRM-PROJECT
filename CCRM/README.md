# Campus Course & Records Manager (CCRM)

## 📌 Project Overview

**Campus Course & Records Manager (CCRM)** is a *Java SE console application* crafted to assist educational institutes in managing:

* **Students**: creation, updates, deactivation, enrollments, transcript management  
* **Courses**: creation, updates, instructor assignment, and stream-based filtering/searching  
* **Enrollment & Grades**: recording marks, GPA calculation, transcript generation  
* **File I/O**: CSV import/export, backups with timestamped directories, recursive utilities

This project showcases *Java OOP concepts*, advanced language features, and design patterns through a functional, real-world example.

---

## ⚙️ How to Run

### Requirements

* JDK 11 or later (tested with JDK 17)  
* IDE like Eclipse or IntelliJ IDEA  
* Git installed (for cloning the repo)  

### Instructions

git clone https://github.com/hawk1411/ccrm-project.git
cd ccrm-project


* Import the project into your IDE as an **Existing Java Project**.  
* Run the main class:

edu.ccrm.cli.CCRMApp


* Follow the interactive menu to navigate through features.

---

## 📚 Java Language Evolution

* **1995**: Initial release (from Oak to Java)  
* **1998 (Java 2)**: Introduced J2SE, J2EE, J2ME editions  
* **2004 (Java 5)**: Generics, enums, annotations, enhanced for-loops  
* **2011 (Java 7)**: NIO.2, try-with-resources, diamond operator  
* **2014 (Java 8)**: Lambdas, Streams API, new Date/Time API  
* **2017 (Java 9)**: Module system introduced  
* **2018+**: Local variable inference (`var`), records, switch expressions  

---

## 🖥️ Java Editions Comparison

| Feature | Java ME             | Java SE                | Java EE (Jakarta EE)              |
|---------|---------------------|------------------------|----------------------------------|
| Scope   | Mobile and embedded | Desktop/general apps   | Enterprise web applications      |
| APIs    | Limited             | Full core Java APIs    | Adds Servlets, JSP, EJB, JPA     |
| Usage   | IoT devices, phones | CLI and desktop apps   | Web servers, distributed systems |
| Example | Mobile games        | *This CCRM project*    | Banking systems                  |

---

## ☕ JDK, JRE, and JVM Explained

* **JDK (Java Development Kit)** — tools for compiling and running Java.  
* **JRE (Java Runtime Environment)** — runtime including JVM and core libraries.  
* **JVM (Java Virtual Machine)** — executes Java bytecode to machine code.  

**Flow**: `.java` file → Compiler → `.class` (bytecode) → JVM execution → machine instructions

---

## 🪟 Install Java on Windows

1. Download the JDK from [Oracle's official site](https://www.oracle.com/java/technologies/downloads/).  
2. Run the installer and set environment variables:


3. Confirm installation:


---

## 🚀 Eclipse Setup

1. Open Eclipse and create a **New Java Project**.  
2. Import source from `src/edu/ccrm`.  
3. Set the run configuration's main class to:


4. Run to see the interactive menu-driven interface.

---

## 📂 Project Structure
<img width="734" height="555" alt="image" src="https://github.com/user-attachments/assets/307c93d6-3893-4fd8-a708-afb4a57ac2f1" />

---

## 🔑 Highlighted Features

* **Encapsulation** — private fields with getters/setters in `Student`  
* **Inheritance & Abstraction** — base class `Person` and derivatives (`Student`, `Instructor`)  
* **Polymorphism** — overridden methods and service interfaces  
* **Immutability** — immutable `CourseCode`  
* **Static Nested Classes** — `Course.Builder`  
* **Inner and Anonymous Classes** — e.g., `ConsoleUtil.bannerPrinter()`  
* **Interfaces** — like `StudentService` and `CourseService`  
* **Enums** — semesters, grades with associated points  
* **Design Patterns** — Singleton (`AppConfig`), Builder (`Course`)  
* **Custom Exceptions** — for business logic validation  
* **Streams & Lambdas** — efficient filtering, searching, reports  
* **Recursion** — utility functions for recursive size calculations  
* **NIO.2 File API** — CSV handling and backup folder creation  
* **Date/Time API** — for enrollment and backup timestamps  

---

## 📊 Concept-to-Code Mapping

| Concept           | Implementing Class/File                                          |
|-------------------|----------------------------------------------------------------|
| Encapsulation     | `Student.java`                                                 |
| Inheritance       | `Person.java`, `Student.java`                                  |
| Abstraction       | `Person.java` (abstract declarations)                         |
| Polymorphism      | Service interfaces and `toString()` overrides                 |
| Singleton         | `AppConfig.java`                                              |
| Builder Pattern   | `Course.Builder`                                              |
| Custom Exceptions | `DuplicateEnrollmentException.java`, `MaxCreditLimitExceededException.java` |
| Streams API       | `CourseServiceImpl.java`                                      |
| Recursion         | `RecursionUtil.java`                                          |
| Date/Time API     | `Student.java`, `Enrollment.java`, `BackupService.java`      |
| File I/O (NIO.2)  | `ImportExportService.java`, `BackupService.java`              |

---

## 🧪 Sample Usage


Example session:

Select an option: 1
Students Menu: 1-Add 2-List 3-Print Profile 4-Back
Enter choice: 1
RegNo: 23BCY10032
Full name: ravi kant mishra
Email: ravi@example.com
DOB (yyyy-mm-dd): 2004-05-18
Student added: Student{id=..., regNo=23bcy10032, ...}

---

## 📂 Data Exports & Backups

* Exported data files saved at:


* Backups created in timestamped folders like:


---

## 🛠️ Java Assertions

Example assertion in `Person.java`:


Enable assertions at runtime using:


---

## 📸 Screenshots

* JDK installation confirmation (`java -version`)  
* Eclipse project import and run setup  
* Running the interactive program  
* Export and backup directory structure  

<img width="1919" height="1020" alt="Screenshot 2025-09-25 165725" src="https://github.com/user-attachments/assets/1185c035-9d61-4301-b3a5-67c6644a9700" />
.

<img width="1338" height="840" alt="Screenshot 2025-09-25 165610" src="https://github.com/user-attachments/assets/35a35daa-71db-41c4-9320-10d726b2401c" />
.
<img width="1919" height="1024" alt="Screenshot 2025-09-25 165553" src="https://github.com/user-attachments/assets/41ab9aaf-8f06-4ac7-b893-786cc8e3bdf5" />
.
<img width="1919" height="1020" alt="Screenshot 2025-09-25 165822" src="https://github.com/user-attachments/assets/06731d1c-037e-4827-b846-368c6aab4ab6" />

.

---

<img width="1919" height="1030" alt="Screenshot 2025-09-25 165925" src="https://github.com/user-attachments/assets/6067b642-15e9-4a6c-8b5c-260a8b0b1e46" />
.


.
<img width="1919" height="1019" alt="Screenshot 2025-09-25 170116" src="https://github.com/user-attachments/assets/fa41d2b2-306c-439f-9736-8708d918a9d2" />
.

## 🙏 Acknowledgements

* Oracle Java official documentation  
* Java SE Tutorials (docs.oracle.com)  
* StackOverflow and community forums  

---











