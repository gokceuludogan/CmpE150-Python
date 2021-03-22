# Frequently Asked Question (FAQ)

1. How can I install the software required for this course?
   * Follow the [Installation Guide](InstallationGuide.md).

2. How can I update Teaching Codes Plugin?
   * Follow the [Teaching Codes Update Guide](TeachingCodesGuide.md)

3. How can I open/submit a project?
   * Follow the [Teaching Codes Guide](TeachingCodesGuide.md)

4. I encountered an error during installation/using Teaching Codes, how can I get help?
   * Check the questions/solutions in this document and then Technical Support Forum on Moodle. If you can't find the solution, send an email to the mail address of your section: cmpe150.mail@gmail.com for CMPE150.01 and cmpe150.mail2@gmail.com for CMPE150.02.

5. I get one of the error listed below while installing Homebrew 

   * curl (6): Could not resolve host: https
   * curl: (1) Protocol ' https not supported or disabled in libcurl

     Try the commands below. If any of them works, then continue installation. When the installation is completed, check it by typing ```brew help```

   * ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"	
     ```

   * ```bash 
     /bin/bash -c "$(curl -fsSL4 https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
     ```

   * ```bash
     /bin/bash -c "$(usr/bin/curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
     ```

   * ```bash
     ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
     ```

6. I can't see the button names in the plugin <a name="button"></a>

   * Change the theme by following these steps:

     * Inside PyCharm, for Windows, click ***File-->Settings***; for MacOS, click ***PyCharm-->Preferences*** and find ***Appearance&Behavior*** on the left. 
     * Go into **Appearance** under ***Appearance&Behavior*** 
     * Change Theme from Intellij Light to something else. (**Darcula** seems fine.)
     * Click **OK**

     ![](figures/ChangeTheme.png)

7. I have deleted the contents of **Main.py** <a name="mainpy"></a>
   * Restore it from **Main.py.txt** under corresponding question's **src** folder

![](figures/Maintxt.png)

8. I can't see the Question description <a name="description"></a>
   * Open the **Question.html** under **WebContent** in a browser
   * Right click on **Question.html** file
   * Click **Open in Browser.** 

<img src="figures/HTML_Browser.png"  style="zoom:50%;" />

9. If there are multiple questions and you see the same description for both questions or still blank page. 

   * Right click on **Question.html** file
   * Choose "**Show in Explorer/Finder**". This step open the folder that contains the html file.

   <img src="figures/HTML_Explorer.png" style="zoom: 50%;" />

   * From the folder, open the html file.

10. I can't see the Exam Results <a name="examresults"></a>

    * Log out, and log in to the Teaching.Codes plugin.	
    * Select the class from the Navigator. Wait a while for the class to load. 
    * Click the ExamResults tab. When you click Open under a question, if nothing is happening:
      * Click the Projects tab on the left of ExamResults
      * Then, go into ExamResults once again. Now, when you click Open, you should be able to see your results. 

