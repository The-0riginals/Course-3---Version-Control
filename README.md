# Version Control by Meta

- This repos contains all of my assignments from the Coursera Course: [Version Control](https://www.coursera.org/learn/introduction-to-version-control?specialization=meta-front-end-developer)

### notes for week 1
- Version Control Systems: distributed version control systems (DVCS) and centralized version control systems (CVCS)
- Git, Mercurial, Subversion, CVS
- Staging vs Production environments
- CI/CD: Continuous Integration, Continuous Delivery, Continuous Deployment



### notes for week 2

- unix: a set of commands that are used to interact with the Unix operating system, it sames as the terminal in mac, linux and the command prompt in windows

- pipe: a way to connect the output of one command to the input of another command
ex:` ls file1.txt |wc-w  `: this command will count the number of words in the file1.txt

- redirection: a way to change where the output of a command goes to, there are 3 types of redirections:
. `>`: standard output, this symbol will redirect the output of a command to a file
. `<`:  standard input, this symbol will redirect the input of a command to a file, 
.`2>`: standard error , this symbol will redirect the error output of a command to a file

ex:  `cat file1.txt > file2.txt`: this command will copy the content of file1.txt to file2.txt
`cat > file1.txt`: this command will create a new file1.txt and will allow you to write in it
`cat < file1.txt`: this command will display the content of file1.txt
`cat -ls > ouptut.txt`: this command will display the content of current folder and will redirect the output to output.txt,if output.txt doesn't exist it will create it
`ls -l /bin/doesntexit 2> error.txt`: this command will take the error output of the ls command and will redirect it to error.txt.

- grep ( global regular expression print ): a command that is used to search for a specific string in a file or multiple files, it can also be used to search for a string in the output of another command
ex: `grep "hello" file1.txt`: this command will search for the string "hello" in file1.txt

`ls -l | grep txt`: this command will search for the string "txt" in the output of the ls command

### git stuffs note for week 3:
staged -> committed -> pushed
The staged area is used to prepare all your files and changes for committing.

- HEAD: a pointer to the most recent commit of the current branch( the branch that you are currently on) with hash-id

- diff: a command that is used to compare two files and display the differences between them, Individual files, branches, and commits can all be compared with Git diff.

- blame: a command that is used to display the last person who modified each line of a file
`git blame <ID><Author><Date><Time><Line number><Content>`
`git blame -L 1,5 file1.txt`: this command will display the last person who modified the lines 1 to 5 of file1.txt

ex: `git blame file1.txt`: this command will display the last person who modified each line of file1.txt

<img src="./Week 3 - Working with Git/git-work-flow.jpg" width=150>