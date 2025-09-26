#Campus Course & Records Manager (CCRM) CCRM is a console-based Java SE application for managing students, courses, enrollments, and academic records. It serves as a comprehensive demonstration of core Java features, Object-Oriented Programming (OOP) principles, and modern software design patterns.

✨ Features Student Management: Add, update, and list all students.

Course Management: Add, search, and list all available courses.

Enrollment & Grading: Enroll students in courses and assign grades.

Transcript Generation: Automatically generate and display a formatted student transcript with GPA calculation.

Data Utilities:

Import data from .csv files.

Export data to .csv files.

Create timestamped backups of data.

Reporting: Generate a GPA distribution report for all students.

🛠️ Tech Stack Language: Java SE (Standard Edition)

Core APIs: Java Streams, Java NIO.2 (for file operations), Java Time API.

🚀 Getting Started Follow these instructions to get a copy of the project up and running on your local machine.

Prerequisites Java Development Kit (JDK): Version 11 or higher is required.

Installation & Execution Clone the Repository

bash git clone cd CCRM Compile the Code From the root CCRM directory, run the following command. This will compile all source files and place them in the bin directory.

bash javac -d bin -sourcepath src src/edu/ccrm/main/MainMenu.java Run the Application Execute the main class from the bin directory using the classpath flag.

bash java -ea -cp bin edu.ccrm.main.MainMenu The -ea flag enables assertions, which are used for validating data like course credits.

📚 Project Documentation

Evolution of Java (Brief Timeline) 1995: Java 1.0 released by Sun Microsystems.
2004: J2SE 5.0 (Tiger) released with major updates like generics and enums.

2014: Java SE 8 released, introducing Lambda Expressions and the Stream API.

2018-Present: Java moves to a faster, 6-month release cycle with Long-Term Support (LTS) versions.

Java Platform Editions: ME vs. SE vs. EE Feature Java ME (Micro Edition) Java SE (Standard Edition) Java EE (Enterprise Edition) Target Platform Resource-constrained devices (IoT). Desktop, server, and console applications. Large-scale, distributed, enterprise applications. Core API A subset of the Java SE API. The core Java platform. Builds on Java SE with additional enterprise APIs. Typical Use Embedded systems. General-purpose programming (this project). Web servers, application servers, microservices.
Java Architecture: JDK, JRE, JVM JVM (Java Virtual Machine): An abstract machine that provides a runtime environment to execute Java bytecode.
JRE (Java Runtime Environment): Includes the JVM and core libraries needed to run Java applications.

JDK (Java Development Kit): A superset of the JRE that includes development tools like the compiler (javac) needed to develop Java applications.

🔧 Syllabus Topic to Code Mapping Topic/Concept File(s) / Location OOP - Encapsulation domain/Student.java (private fields, public getters/setters) OOP - Inheritance domain/Student.java extends domain/Person.java OOP - Abstraction domain/Person.java (abstract class with abstract methods) OOP - Polymorphism service/TranscriptService.java (uses Person reference for Student) Design Pattern: Singleton config/AppConfig.java Design Pattern: Builder domain/Course.java (implemented via CourseBuilder) NIO.2 API (Path, Files) io/BackupService.java Streams API service/CourseService.java (for search/filter) Lambdas & Functional I/F util/Comparators.java Recursion util/RecursiveFileUtils.java Custom Exceptions exception/DuplicateEnrollmentException.java 📂 Project Structure The project is organized into a clear, package-based structure within the src directory:

text src/ └── edu/ └── ccrm/ ├── config/ # Application configuration classes ├── domain/ # Core business entities (Student, Course, etc.) ├── exception/ # Custom exception classes ├── io/ # Input/output operations (file handling) ├── main/ # Main application entry point ├── service/ # Business logic services └── util/ # Utility classes and helpers 👨‍💻 Developer SHIVENDRA SINGH
