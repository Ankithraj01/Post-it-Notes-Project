# Post-it-Notes-Project

The Pin Your Notes application is a GUI-based note-taking application that allows users to create, view, edit, and delete notes. The application uses the sqlite3 module to create a database and store notes.

Explanation
The Pin Your Notes application is a GUI-based note-taking application that allows users to create, view, edit, and delete notes. The application uses the sqlite3 module to create a database and store notes.

The application window is created using the Tk class from the tkinter module. The window is set to a size of 700x600 pixels and titled "Pin Your Notes". A label with the text "Post-it Note" is added to the window using the Label widget.

The sqlite3 module is used to create a database connection and connect to a table named notes_table. If the table does not exist, it is created. The notes_table has two columns: notes_title and notes.

The application has four functions: create_notes(), view_notes(), edit_notes(), and delete_notes().

The create_notes() function obtains the input values for notes_title and notes from the user. If both values are missing, a prompt is raised. If both values are present, the values are inserted into the notes_table using an SQL INSERT statement. A prompt is raised to confirm that the note has been added. The changes are committed to the database.

The view_notes() function obtains the input value for notes_title from the user. If no input is given, all notes are retrieved using an SQL SELECT statement. If a title is given, notes matching the title are retrieved using an SQL SELECT statement. The retrieved notes are displayed in a prompt using the messagebox.showinfo() method.

The edit_notes() function obtains the input values for notes_title and notes from the user. If both values are missing, a prompt is raised. If both values are present, the notes value is updated in the notes_table using an SQL UPDATE statement. A prompt is raised to confirm that the note has been edited and saved. The changes are committed to the database.

The delete_notes() function obtains the input value for notes_title from the user. If no input is given, a prompt is raised to enter details. If a title is given, notes matching the title are deleted using an SQL DELETE statement. A prompt is raised to confirm that the note(s) have been deleted. The changes are committed to the database.

