# **Setting Up Jupyter Notebook**  
There are two main approaches:  
1. The Easy Way > **Anaconda** 
2. The Lightweight Way > **Pip** via Command Line  (better option for laptop)

### **Anaconda**  
Best for Beginners, Data Science, Machine Learning.  
**Pros**: Installs Python, Jupyter, and hundreds of popular libraries all at once.  
**Cons**: Large download size (\~1 GB).  

### **Pip**  
Best for Developers who like to keep their system lean.  
**Pros**: Lightweight, fast installation, you only install what you need.  
**Cons**: Requires you to already have Python installed and use the command line.  

<br>

## **Installing via Pip**

If you already have Python installed and prefer using your terminal/command prompt, you can install Jupyter directly using Python's package manager, pip.

### **Step-by-Step Implementation**

1. Ensure your package installer is up to date by running  
**`$ pip install --upgrade pip`**  
2. NOTE: you might need to enable Windows Long Path support to overcome the error caused by Windows default of a 260-character limit for file paths.  
   * Click your Windows Start menu, type PowerShell, right-click it, and select Run as administrator.
   * Copy and paste the following command into the PowerShell window, then press Enter:  
**`New-ItemProperty -Path "HKLM:\\System\\CurrentControlSet\\Control\\FileSystem" -Name "LongPathsEnabled" -Value 1 -PropertyType DWORD -Force`**
   * Close the PowerShell window.
3. Install the classic Jupyter Notebook  
**`$ pip install notebook`**  
4. Add Jupyter directory to PATH  
   * Press the Windows Key on your keyboard, type "environment variables", and select Edit the system environment variables.
   * A small System Properties window will pop up. Click the Environment Variables... button near the bottom right.
   * In the new window, look at the top section labeled User variables for gio. Find the variable named Path (or PATH), click on it to highlight it, and click Edit....
   * A list of paths will appear. Click the New button on the right side.
   * Paste the path you copied earlier into the blank line that appears.
   * Click OK on the Edit window, click OK on the Environment Variables window, and click OK on the System Properties window to save your changes.
5. Launch it at any time by typing this command into your terminal  
**`$ jupyter notebook`**  

