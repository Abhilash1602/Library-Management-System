# Library Management System

This project implements a Library Management System using Object-Oriented Programming (OOP) concepts such as class inheritance, data abstraction, and other design principles.

## Object-Oriented Design Concepts

### Class Inheritance

- **LibraryItem**: This is an abstract base class that defines the common interface for all library items. It includes a pure virtual function `printDetails()` that must be implemented by all derived classes.
- **Book, Journals, PublicationRank**: These classes inherit from `LibraryItem` and implement the `printDetails()` function. They also include additional attributes and methods specific to each type of library item.

### Data Abstraction

- **LibraryItem**: By defining a common interface for all library items, the details of each specific type of item are hidden from the rest of the system. This allows the system to treat all library items uniformly.
- **User**: This class encapsulates the details of a library user, including their name, whether they are a teacher, and the books they have borrowed. The internal details of how these attributes are managed are hidden from the rest of the system.

### Other OOP Concepts

- **Encapsulation**: Each class encapsulates its data and provides public methods to interact with that data. For example, the `Book` class has private attributes such as `title` and `authors`, and public methods such as `getTitle()` and `setTitle()`.
- **Polymorphism**: The `LibraryItem` class defines a virtual function `printDetails()`, which is overridden by each derived class. This allows the system to call `printDetails()` on a `LibraryItem` pointer and have the correct function executed based on the actual type of the object.

## Commands to Run the Makefile and See the Output

### Step 1: Compile the Code

Open a terminal and navigate to the directory containing the Makefile. Run the following command to compile the code:

```sh
mingw32-make
```

### Step 2: Run the Output

After successful compilation, run the generated executable to see the output:

```sh
.\Output.exe
```

### Step 3: Clean the Build

To clean the build and remove the generated object files and executable, run:

```sh
mingw32-make clean
```

## File Structure

- **main.cpp**: The main entry point of the application. It initializes the library, reads data from CSV files, and provides a menu for user interaction.
- **Library.cpp**: Contains the `Library` class, which manages the collection of library items and users.
- **Book.cpp, Journals.cpp, PublicationRank.cpp**: Define the `Book`, `Journals`, and `PublicationRank` classes, respectively.
- **User.cpp**: Defines the `User` class, which represents a library user.
- **functions.cpp**: Contains utility functions used throughout the application.
- **LibraryItem.cpp**: Defines the abstract base class `LibraryItem`.

## Conclusion

This project demonstrates the use of OOP concepts to build a flexible and maintainable Library Management System. By leveraging class inheritance, data abstraction, encapsulation, and polymorphism, the system is able to manage different types of library items and users in a uniform and efficient manner.

```

```
