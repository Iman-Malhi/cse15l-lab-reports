# LAB REPORT 3!
Consider the command `find`.
First, I used the `find -iname` command.
Example 1:
<code><pre>find -iname "chapter-*.txt"
./technical/911report/chapter-1.txt
./technical/911report/chapter-10.txt
./technical/911report/chapter-11.txt
./technical/911report/chapter-12.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-2.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-5.txt
./technical/911report/chapter-6.txt
./technical/911report/chapter-7.txt
./technical/911report/chapter-8.txt
./technical/911report/chapter-9.txt`
Example 2:
`find -iname "1468-6708-3-*.txt"
./technical/biomed/1468-6708-3-1.txt
./technical/biomed/1468-6708-3-10.txt
./technical/biomed/1468-6708-3-3.txt
./technical/biomed/1468-6708-3-4.txt
./technical/biomed/1468-6708-3-7.txt`
Then I used the `find -type` command.
Example 1:
`find -type d
.
./lib
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/government/About_LSC
./technical/government/Alcohol_Problems
./technical/government/Env_Prot_Agen
./technical/government/Gen_Account_Office
./technical/government/Media
./technical/government/Post_Rate_Comm
./technical/plos</code></pre>
Example 2:
`find -type f -empty`
Then I used the `find -maxdepth` command.
Example 1: 
`find -maxdepth 1 -type d
.
./lib
./technical`
Example 2:
`find -maxdepth 2 -type f 
./DocSearchServer.java
./README.md
./Server.java
./TestDocSearch.java
./lib/hamcrest-core-1.3.jar
./lib/junit-4.13.2.jar`
And finally, I used the `find -ipath` command.
Example 1:
`find -ipath "*chapter-1.txt*"
./technical/911report/chapter-1.txt`
Example 2:
find -ipath "*Annual_Fee.txt*"
./technical/government/Media/Annual_Fee.txt
