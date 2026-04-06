# Library Management System - Java

## Complete Java Syllabus Coverage (Unit 1-5)

### Project Structure
```
src/com/library/
├── LibraryManagementSystem.java    (Main Application)
├── model/                          (Unit 1: OOP - Classes, Inheritance, Serialization)
│   ├── Person.java                 (Abstract class - Inheritance)
│   ├── Book.java                   (Encapsulation, Serializable, Comparable)
│   ├── Member.java                 (Extends Person - Inheritance)
│   └── Transaction.java            (Business entity)
├── interfaces/                     (Unit 1: Interfaces)
│   ├── LibraryOperations.java
│   ├── Searchable.java
│   └── Reportable.java
├── exceptions/                     (Unit 1: Exception Handling)
│   ├── LibraryException.java       (Base exception)
│   ├── BookNotFoundException.java  (Custom exception)
│   ├── MemberNotFoundException.java
│   ├── BookNotAvailableException.java
│   └── MaxBooksExceededException.java
├── service/                        (Business Logic)
│   └── LibraryService.java         (Try-Catch-Finally, Throws)
├── threading/                      (Unit 1: Threading)
│   ├── BookSearchThread.java       (extends Thread)
│   ├── OverdueCheckerRunnable.java (implements Runnable)
│   └── ThreadDemo.java             (Thread Life Cycle demo)
├── io/                             (Unit 1: I/O & Serialization)
│   └── FileHandler.java            (Object Serialization, Text I/O)
├── beans/                          (Unit 2: JavaBeans)
│   ├── BookBean.java               (JavaBean with all property types)
│   ├── BookBeanInfo.java           (BeanInfo class)
│   ├── BookBeanDemo.java           (Bound, Constrained, Indexed properties)
│   ├── LibraryEvent.java           (Custom Event)
│   └── LibraryEventListener.java   (Custom Event Listener)
├── database/                       (Unit 3: JDBC)
│   ├── DatabaseConfig.java         (JDBC configuration)
│   ├── DatabaseManager.java        (CRUD, Transactions, Type Mapping)
│   └── ConnectionPool.java         (Connection Pooling)
├── gui/                            (Unit 4: Swing)
│   └── LibraryMainFrame.java       (Complete Swing GUI)
├── applet/                         (Unit 5: Applets)
│   ├── LibraryApplet.java          (Applet basics, Multimedia, URL)
│   └── LibraryApplet.html          (Applet HTML tags)
├── networking/                     (Unit 5: Networking)
│   ├── LibraryServer.java          (Socket server)
│   └── LibraryClient.java          (Socket client)
├── rmi/                            (Unit 5: RMI)
│   ├── LibraryRemote.java          (Remote interface)
│   └── LibraryRemoteImpl.java      (Remote implementation)
├── servlet/                        (Unit 5: Servlets)
│   ├── LibraryServlet.java         (Servlet API)
│   └── web.xml                     (Web deployment descriptor)
└── ejb/                            (Unit 5: EJB)
    ├── LibrarySessionBean.java     (Stateless Session Bean)
    ├── LibraryEntityBean.java      (Entity Bean / JPA Entity)
    └── LibraryMessageBean.java     (Message-Driven Bean)
```

### Syllabus Topics Covered

| Unit | Topic | Files |
|------|-------|-------|
| 1 | Classes, Objects, Access Modifiers | model/*.java |
| 1 | Interfaces | interfaces/*.java |
| 1 | Inheritance | Person.java, Member.java |
| 1 | Arrays, Packages | Throughout project |
| 1 | Exception Handling (Try/Catch/Finally/Throws) | exceptions/*.java, LibraryService.java |
| 1 | Multithreading, Thread Life Cycle | threading/*.java |
| 1 | I/O and Object Serialization | io/FileHandler.java |
| 2 | JavaBeans Component Model | beans/BookBean.java |
| 2 | Property Types (Simple, Bound, Constrained, Indexed, Boolean) | beans/BookBean.java |
| 2 | BeanInfo Classes | beans/BookBeanInfo.java |
| 2 | Custom Events | beans/LibraryEvent.java, LibraryEventListener.java |
| 2 | GUI / Event Model | gui/LibraryMainFrame.java |
| 3 | JDBC Drivers, java.sql API | database/DatabaseManager.java |
| 3 | SQL to Java Type Mapping | database/DatabaseManager.java |
| 3 | Coding Transactions | database/DatabaseManager.java |
| 3 | Connection Pooling | database/ConnectionPool.java |
| 4 | Swing MVC, Layout Managers | gui/LibraryMainFrame.java |
| 4 | Text Input, Choice Components | gui/LibraryMainFrame.java |
| 4 | Menus, Toolbars, Tooltips | gui/LibraryMainFrame.java |
| 4 | Dialog Boxes, Tabbed/Split Panes | gui/LibraryMainFrame.java |
| 4 | Tables, Progress Bars | gui/LibraryMainFrame.java |
| 5 | Applets, HTML Tags, URL | applet/*.java |
| 5 | Socket Programming | networking/*.java |
| 5 | RMI | rmi/*.java |
| 5 | Servlets, Servlet API | servlet/*.java |
| 5 | Session EJBs, Entity EJBs, MDB | ejb/*.java |

### How to Compile & Run

```bash
# Compile all files
javac -d bin src/com/library/**/*.java src/com/library/*.java

# Run with GUI + Console demos
java -cp bin com.library.LibraryManagementSystem

# Run console only
java -cp bin com.library.LibraryManagementSystem console

# Run GUI only
java -cp bin com.library.LibraryManagementSystem gui
```

### Requirements
- Java JDK 8 or higher
- MySQL (for JDBC features - optional)
- Servlet container like Tomcat (for Servlet features - optional)
- EJB container like WildFly (for EJB features - optional)
