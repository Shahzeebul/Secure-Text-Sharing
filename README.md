# Secure-Text-Sharing
The provided Python code creates a simple GUI application for secure text sharing using the Tkinter library and Fernet encryption from the cryptography module. Below is a breakdown of the code:

1. Import Necessary Modules:
   - The code starts by importing the required modules, including `tkinter` for GUI, `ttk` for themed widgets, and `cryptography.fernet` for Fernet encryption.

2. Functions:
   - `encrypt_text()`: Handles the encryption of the input text, generates a Fernet key, encrypts the text, saves it to a file, and displays the generated key.
   - `show_decrypted_text()`: Retrieves the Fernet key from the entry field, decrypts the previously encrypted text from the file, and displays the decrypted text in a new themed Tkinter window.
   - `save_to_file(data, filename)`: Saves data to a specified file.
   - `load_from_file(filename)`: Loads data from a specified file.

3. Main Themed Tkinter Window:
   - Creates the main Tkinter window using `ThemedTk` from the `ttkthemes` module.
   - Sets the theme to "radiance" and the window title to "Secure Text Sharing."

4. GUI Elements:
   - Labels, text widgets, buttons, and entry fields are created using `ttk.Label`, `tk.Text`, `ttk.Entry`, and `ttk.Button`.
   - The GUI elements are configured and packed into the window for display.

5. Styling:
   - `ttk.Style()` is used to create a style for ttk widgets, and text and button colors are configured.

6. Event Handling:
   - The "Encrypt" button is associated with the `encrypt_text()` function, and the "Show Decrypted Text" button is associated with the `show_decrypted_text()` function.

7. Main Loop:
   - `window.mainloop()` starts the Tkinter main loop for the main window, allowing user interaction.

Note: Ensure that you have the required libraries (`tkinter`, `ttkthemes`, `cryptography`) installed before running the code. Additionally, this code provides a basic structure, and you may need to enhance it based on your specific requirements and security considerations.
