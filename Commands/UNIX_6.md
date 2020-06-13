
<h2>quota</h2>
To check your current quota and how much of it you have used, type <b>% quota -v</b>


<h2>df</h2>
The <b>df</b> command reports on the space left on the file system. For example, to find out how much space is left on the fileserver, type <b>% df .</b>


<h2>du</h2>
The <b>du</b> command outputs the number of kilobytes used by each subdirectory. Useful if you have gone over quota and you want to find out which directory has the most files. In your home-directory, type <b>% du -s *</b>

(The -s flag will display only a summary (total size) and the * means all files and directories.)


<h2>gzip</h2>
This reduces the size of a file, thus freeing valuable disk space. For example, type <b>% ls -l gudi.txt</b> and note the size of the file using ls -l . Then to compress gudi.txt, type <b>% gzip gudi.txt</b> .....This will compress the file and place it in a file called gudi.txt.gz

To see the change in size, type ls -l again........To expand the file, use the gunzip command 
<b>% gunzip gudi.txt.gz</b>


<h2>zcat</h2>
<b>zcat</b> will read gzipped files without needing to uncompress them first. So, type <b>% zcat gudi.txt.gz</b>

( If the text scrolls too fast for you, pipe the output though less . <b>% zcat science.txt.gz | less</b> )


<h2>file</h2>
<b>file</b> classifies the named files according to the type of data they contain, for example ascii (text), pictures, compressed data, etc.. To report on all files in your home directory, type <b> % file *</b>


<h2>diff</h2>
This command compares the contents of two files and displays the differences. Suppose you have a file called file1 and you edit some part of it and save it as file2. To see the differences type <b>% diff file1 file2</b>
(Lines beginning with a < denotes file1, while lines beginning with a > denotes file2.)


<h2>find</h2>
This searches through the directories for files and directories with a given name, date, size, or any other attribute you care to specify. It is a simple command but with many options - you can read the manual by typing man find. To search for all fies with the extention .txt, starting at the current directory (.) and working through all sub-directories, then printing the name of the file to the screen, type <b>% find . -name "*.txt" -print</b>

To find files over 1Mb in size, and display the result as a long listing, type <b>% find . -size +1M -ls</b>


<h2>history</h2>
The C shell keeps an ordered list of all the commands that you have entered. Each command is given a number according to the order it was entered.
<b>% history (show command history list)</b>

More about this, refer the <b>link :</b>

# http://www.ee.surrey.ac.uk/Teaching/Unix/unix6.html


 
