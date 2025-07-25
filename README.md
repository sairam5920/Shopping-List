#Shopping List 

This Shopping List Manager is a beginner-friendly Java console application that allows users to maintain a simple shopping list using file I/O operations. 
It reads an existing list from a file (data.txt), displays the current items, and allows the user to add a new item via console input. The updated list is
then saved back to the file, ensuring persistent data between runs. The program uses ArrayList for dynamic storage, Scanner for reading both user and file 
input, and PrintWriter for writing to the file. This project showcases basic file handling, user interaction, and list manipulation in Java—ideal for those
learning how to persist data locally.

🔹 main(String[] args)
Purpose: This is the entry point of the program.

What it does:

Calls readData() to load the existing shopping list from data.txt.

Displays the current list using printList().

Prompts the user to add a new item.

Adds the new item to the list.

Saves the updated list using writeData().

🔹 readData() : ArrayList<String>
Purpose: Reads shopping list items from the file data.txt.

Returns: An ArrayList<String> containing the items read from the file.

Details:

Opens the file using a Scanner.

Reads each line and adds it to the list.

Handles the case where the file doesn't exist (prints: "No List Exists.").

🔹 writeData(ArrayList<String> list)
Purpose: Writes the current shopping list to the file data.txt.

Parameters: list — the list of items to be saved.

Details:

Opens the file using PrintWriter.

Writes each item in the list to a new line in the file.

Handles IOException if writing fails (prints: "Unable to write").

🔹 printList(ArrayList<String> l)
Purpose: Prints the current shopping list to the console.

Parameters: l — the list of items to display.

Details:

Checks if the list is non-empty.

Prints "Current Shopping List:" followed by each item on a new line.

