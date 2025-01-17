
---

**DoLess**  
**Why work harder when you can DoLess?**  

What is DoLess?  
DoLess is a Python package designed for developers who want to avoid repetitive workflows, clunky threading, or verbose browser automation. It provides shortcuts for tasks like handling files, automating websites, and managing threads with ease.  

---

Features:  
1. **Thread Management**:  
   - Execute tasks in parallel with simple threading.  
   - Includes an animated load buffer to make you look productive.  

2. **Browser Automation**:  
   - Headless browsing, form filling, and button clicking.  
   - Easy parsing of links, buttons, and login forms.  

3. **File Handling**:  
   - Check file existence, create files, append content, and overwrite efficiently.  

4. **Console Tricks**:  
   - Clear the console, print centered text, or enumerate lists stylishly.  

---

Installation:  
Install DoLess directly from GitHub using pip:  

```
pip install git+https://github.com/Casbian/DoLess.git
```  

This command installs DoLess directly from the repository to ensure you get the latest version.  

---

Quickstart Guide:  

1. **Master Multithreading**  
   Let DoLess handle thread management for you:  

   ```python
   from DoLess.threads import SubmitTasktoThreadWITHLoadBuffer

   def my_task():  
       print("Doing some important stuff...")

   SubmitTasktoThreadWITHLoadBuffer(my_task)
   ```  

   Effortless threading with built-in buffering.  

2. **Browser Automation**  
   Automate web tasks with minimal effort:  

   ```python
   from DoLess.web import StartBrowser, GoToUrl, ParseforLinks

   StartBrowser()  
   GoToUrl("https://example.com")  
   http_links, https_links = ParseforLinks()  
   print("HTTP Links:", http_links)  
   print("HTTPS Links:", https_links)
   ```  

3. **Handle Files**  
   Simplify file operations:  

   ```python
   from DoLess.files import CheckFileExistence, CreateFile, AppendtoFile

   file_name = "example.txt"

   if not CheckFileExistence(file_name):  
       CreateFile(file_name)  

   AppendtoFile(file_name, "This is a line of text!")
   ```  

4. **Console Wizardry**  
   Keep your console clean and professional:  

   ```python
   from DoLess.console import ClearConsole, CenteredPrint

   ClearConsole()  
   CenteredPrint("Welcome to DoLess!", "*")
   ```  

---

Contributing:  
Want to add a feature or fix a bug? Contributing is simple:  

1. Fork the repository.  
2. Clone it:  
   `git clone https://github.com/Casbian/DoLess.git`  
3. Make your changes.  
4. Submit a pull request.  

---

License:  
DoLess is licensed under the MIT License. Feel free to share, remix, and improve it!  

---