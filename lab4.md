# LAB REPORT 4 #
**Step 4:**

Logged into ieng6 by typing ssh cs15lsp23mi@ieng6.ucsd.edu (not in vim yet).
![image](step4.png)

**Step 5:**

Entered vim mode by entering the command vim tutor. Entered :!git clone https://github.com/Iman-Malhi/lab7.git <enter>.
![image](step5.png)

**Step 6:**

:!javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar ListExamples.java ListExamplesTests.java <enter> :!java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests <enter>
![image](step6b.png)
  
**Step 7:**

:e ListExamplesTests.java <delete> 2 (enter 2 to replace 1 in code shown below) <escape> :w
![image](step6.png)

**Step 8:**

:!javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar ListExamples.java ListExamplesTests.java <enter> :!java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests <enter>
![image](step7.png)
  
**Step 9:**
  
:!git add --all 
:!git commit -m "hi"
:!git push origin
![image](step8.png)
