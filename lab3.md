# LAB REPORT 3
Consider the command `find`. I found about the following command-line options through the website [Red Hat](https://www.redhat.com/sysadmin/linux-find-command).

First, I used the `find -iname` command.

**Example 1:**
<pre><code>find -iname "chapter-*.txt"
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
./technical/911report/chapter-9.txt`</code></pre>

In the above example, `find -iname` does a partial search for files are of the format `chapter-*.txt`, the `*` can be replaced by any character(s) (some examples above would be `1`, `12`, and `9`. This command would be helpful for doing a non-exact search, where you want to find similarily named files instead of one exact file.

**Example 2:**
<pre><code>find -iname "1468-6708-3-*.txt"
./technical/biomed/1468-6708-3-1.txt
./technical/biomed/1468-6708-3-10.txt
./technical/biomed/1468-6708-3-3.txt
./technical/biomed/1468-6708-3-4.txt
./technical/biomed/1468-6708-3-7.txt</code></pre>

In the above example, `find -iname` does a partial search for files are of the format `1468-6708-3-*.txt`, the `*` can be replaced by any character(s) (some examples above would be `1`, `10`, and `7`. As stated earlier, the `find -iname` command would be helpful for doing a non-exact search, where you want to find similarily named files instead of one exact file.

Then I used the `find -type` command.

**Example 1:**
<pre><code>find -type d
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

In the above example, `find -type d` lists all the directories as a path (does a search of the type "directory" and returns in the terminal). This can be helpful if the user needs to paths to all the directories.

**Example 2:**
<pre><code>find -type f -empty</code></pre>

In the above example, `find -type f -empty` lists all the files that are empty. the `-type f` part of the command tells the computer that its looking for files, and the `-empty` part of the command tells the computer it is looking for files that are empty (the above example returned nothing which tells us there are no empty files). This can be helpful if the user is looking for empty files, maybe with the intent on deleting them.

Then I used the `find -maxdepth` command.

**Example 1:**
<pre><code>find -maxdepth 1 -type d
.
./lib
./technical</code></pre>

`find -maxdepth 1 -type d` finds a limited amount of directories and returns them; specifically, `-maxdepth` makes the command return the number of searches equivalent to the max depth(not including the starting point). This command can be helpful for limiting the amount of searches `find` does.

**Example 2:**
<pre><code>find -maxdepth 2 -type f 
./DocSearchServer.java
./README.md
./Server.java
./TestDocSearch.java
./lib/hamcrest-core-1.3.jar
./lib/junit-4.13.2.jar</code></pre>

`find -maxdepth 2 -type f` finds a limited amount of files and returns them; as stated earlier, `-maxdepth` makes the command return the number of searches equivalent to the max depth (not including the starting point). This command can be helpful for limiting the amount of searches `find` does.

And finally, I used the `find -ipath` command.

**Example 1:**
<pre><code>find -ipath "*chapter-1.txt*"
./technical/911report/chapter-1.txt</code></pre>

`find -ipath "*chapter-1.txt*"` returns the path of a file, in this case the `chapter-1.txt` file. This can be helpful for finding specific paths of specific files, allowing the user to know the location of said file.  

**Example 2:**
<pre><code>find -ipath "*Annual_Fee.txt*"
./technical/government/Media/Annual_Fee.txt</code></pre>

`find -ipath ""*Annual_Fee.txt*"` returns the path of a file, in this case the `Annual_Fee.txt file`. This can be helpful for finding specific paths of specific files, allowing the user to know the location of said file.  


