MiniShelf: Personal Book Record System – Project Information

Members:
        Jerome Lontoc
        Rey Magramo
        James Getulle




Users can:
	1. Add Book
	2. View All Books
	3. Search Book
	4. Mark as Read / Unread
	5. Delete Book
	6. Exit




Project Overview

    MiniShelf is a console-based Java program that works like a small personal book record system. The goal of the project is to help users store books, check them, search them, and update their reading status. The system uses basic object-oriented programming ideas so the code stays clean and easy to update.

    The program has three types of books: novels, magazines, and textbooks. Each one has details like title, pages, and author or publisher. The user can add books, view all stored books, search by title, mark books as read or unread, and delete books. Everything is done through a simple menu in the console.




OOP Concepts Used

    Encapsulation
        All book details are private inside the Book class.
        Getters and setters manage access.
        This keeps the data safe and avoids wrong changes.

    Inheritance
        Novel, Magazine, and Textbook all extend the base Book class.
        Each type adds its own field like genre, issue month, or subject.

    Polymorphism
        Each subclass overrides the getDetails() method.
        This helps show extra info depending on the book type.

    Abstraction
        The Book class holds common data and methods for all books.
        Subclasses only add what is different from other book types.

    Exception Handling
        try-catch is used when reading numbers.
        This keeps the program from crashing when the user enters wrong input.





Program Structure

    Main Classes

    Book (base class)
        Stores shared details like title, pages, author or publisher, and read status.

    Novel (subclass)
        Adds a genre field and overrides the detail display.

    Magazine (subclass)
        Adds an issue month field.

    Textbook (subclass)
        Adds a subject field.

    MiniShelf (main class)
        Handles the menu, book list, and all user actions.




Text-Based Class Diagram

                +----------------------+
                |        Book          |
                +----------------------+
                | - title              |
                | - authorOrPublisher  |
                | - pages              |
                | - isRead             |
                | - type               |
                +----------------------+
                | + getDetails()       |
                +----------+-----------+
                           |
       ------------------------------------------------
       |                         |                    |
+--------------+        +----------------+    +----------------+
|    Novel     |        |   Magazine     |    |   Textbook     |
+--------------+        +----------------+    +----------------+
| + genre      |        | + issueMonth   |    | + subject      |
| overrides    |        | overrides      |    | overrides      |
+--------------+        +----------------+    +----------------+

                     +------------------------+
                     |       MiniShelf        |
                     +------------------------+
                     | main program logic     |
                     | array of Book objects  |
                     +------------------------+




How to Run the Program

	Save the Java file
		Make sure the name is MiniShelf.java.

	Open Command Prompt / Terminal
		Go to the folder with the file.
		cd path\to\project

	Compile
		javac MiniShelf.java

	Run
		java MiniShelf

	Use the Menu
		You can:

		Add books

		See all books

		Search by title

		Mark a book as read or unread

		Delete a book






Sample Output
    === MiniShelf: Personal Book Record System ===
    1. Add Book
    2. View All Books
    3. Search Book by Title
    4. Mark as Read / Unread
    5. Delete Book
    6. Exit
    Enter choice:




Future Enhancements

    Better Interface
        Add colors or move the program to a GUI like JavaFX.

    More Features
        Sorting, filtering, and saving the book list to a file.

    Data Storage
        Use a database or text file so books stay saved even after closing.





Contributors
	Jerome Lontoc - Leader, Console Programming
	Rey Magramo - Researcher, Writer
	James Getulle - File Handling 




Acknowledgement

	We, the group of "Triple Trouble", sincerely express our gratitude to our instructor Ms. Cristiana Grace Alib for the guidance and support all throughout the completion of this project. We also appreciate our classmates and group members for helping each other and cooperation during the development process.

