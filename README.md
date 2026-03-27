# File-Based-Notes-Saver---python
To design and implement a Notes Saver Application using Python.  The system allows the user to add and view notes, storing them in a file for future  access. 
# 📝 Notes Saver Application (Python)

A simple and efficient **Notes Saver Application** built using Python.  
This project allows users to add and view notes, storing them in a file for future access.

---

## 🚀 Features

- 📌 Add notes and save them permanently
- 📖 View all saved notes
- 💾 Stores data in a text file (`notes.txt`)
- ⚠️ Handles file errors using exception handling
- 🔁 Menu-driven program for continuous use

---

## 🛠️ Technologies Used

- Python 3
- File Handling
- Exception Handling
- Functions & Loops

---

## 📂 Project Structure


📁 Notes-Saver/
│── main.py
│── notes.txt (auto-created)


---

## ▶️ How to Run

1. Install Python (3.x)
2. Save the code in a file named `main.py`
3. Run the program:

```bash
python main.py
📌 Usage

After running the program:

📌 Notes Saver Menu
1. Add Note
2. View Notes
3. Exit
Enter 1 → Add a note
Enter 2 → View saved notes
Enter 3 → Exit
💻 Source Code
def write_note():
    note = input("📝 Enter your note: ")
    
    with open("notes.txt", "a") as file:
        file.write(note + "\n")
    
    print("✅ Note saved successfully!")

def read_notes():
    try:
        with open("notes.txt", "r") as file:
            content = file.read()
            
            if content.strip() == "":
                print("📭 No notes found.")
            else:
                print("\n📒 Your Notes:\n")
                print(content)
    except FileNotFoundError:
        print("❌ No notes file found. Please add a note first.")

def main():
    while True:
        print("\n📌 Notes Saver Menu")
        print("1. Add Note")
        print("2. View Notes")
        print("3. Exit")

        choice = input("Enter your choice (1-3): ")

        if choice == "1":
            write_note()
        elif choice == "2":
            read_notes()
        elif choice == "3":
            print("👋 Exiting... Goodbye!")
            break
        else:
            print("⚠️ Invalid choice. Try again.")

# Run the program
main()
<img width="1918" height="730" alt="1" src="https://github.com/user-attachments/assets/726701a0-3cf4-4ca8-9c43-8acfcf4bfaac" />

💡 Sample Output
📌 Notes Saver Menu
1. Add Note
2. View Notes
3. Exit

Enter your choice: 1
📝 Enter your note: Study Python
✅ Note saved successfully!
Enter your choice: 2

📒 Your Notes:

Study Python
🧠 Learning Outcomes
Learned file handling in Python
Implemented exception handling
Built a menu-driven program
Practiced modular coding using functions
🔮 Future Enhancements
✏️ Edit/Delete notes feature
⏰ Add timestamp to notes
🎨 GUI using Tkinter
🗄️ Database integration
👩‍💻 Author

Shalini U
B.Tech Artificial Intelligence & Data Science

⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!


---

If you want it to look even more 🔥 on GitHub:
- I can add **badges + project preview images**
- Or help you **push this repo step-by-step**

Just tell me 👍
