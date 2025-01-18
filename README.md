
---

**CoreEase**  
**Why work harder when you can CoreEase?**

### What is CoreEase?  
CoreEase is a Python package designed for developers who want to avoid repetitive workflows, clunky threading, or verbose browser automation. It provides shortcuts for tasks like handling files, automating websites, and managing threads with ease.

---

### Features:  
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

### Installation:  
You can now install CoreEase directly from **PyPI** using pip:

```
pip install CoreEase
```  

Alternatively, if you want to install directly from GitHub to get the latest version:

```
pip install git+https://github.com/Casbian/CoreEase.git
```  

After uploading to **PyPI**, users will be able to install the package directly from there. 

---

### Quickstart Guide:

1. **Master Multithreading**  
   Let CoreEase handle thread management for you:  

   ```python
   from CoreEase.threads import SubmitTasktoThreadWITHLoadBuffer

   def my_task():  
       print("Doing some important stuff...")

   SubmitTasktoThreadWITHLoadBuffer(my_task)
   ```  

   Effortless threading with built-in buffering.

2. **Browser Automation**  
   Automate web tasks with minimal effort:  

   ```python
   from CoreEase.web import StartBrowser, GoToUrl, ParseforLinks

   StartBrowser()  
   GoToUrl("https://example.com")  
   http_links, https_links = ParseforLinks()  
   print("HTTP Links:", http_links)  
   print("HTTPS Links:", https_links)
   ```  

3. **Handle Files**  
   Simplify file operations:  

   ```python
   from CoreEase.files import CheckFileExistence, CreateFile, AppendtoFile

   file_name = "example.txt"

   if not CheckFileExistence(file_name):  
       CreateFile(file_name)  

   AppendtoFile(file_name, "This is a line of text!")
   ```  

4. **Console Wizardry**  
   Keep your console clean and professional:  

   ```python
   from CoreEase.console import ClearConsole, CenteredPrint

   ClearConsole()  
   CenteredPrint("Welcome to CoreEase!", "*")
   ```  

---

### Contributing:  
Want to add a feature or fix a bug? Contributing is simple:

1. Fork the repository.  
2. Clone it:  
   `git clone https://github.com/Casbian/CoreEase.git`  
3. Make your changes.  
4. Submit a pull request.  

---

### License:  
CoreEase is licensed under the MIT License. Feel free to share, remix, and improve it!

---
