# Filter-with-grep

<h2>Activity overview</h2>

In this lab activity, I’ll use the ```grep``` command and piping to search for files and to return specific information from files.

As a security analyst, it’s key to know how to find the information I need. The ability to search for specific strings can help me locate what I need more efficiently.

<h2>Scenario</h2>

In this scenario, I need to obtain information contained in server log and user data files. I also need to find files with specific names.

Here’s how I’ll do this: First, I’ll navigate to the ```logs``` directory and return the error messages in the ```server_logs.txt``` file. Next, I’ll navigate to the ```users``` directory and search for files that contain a specific string in their names. Finally, I’ll search for information contained in user files.

<h2>Task 1. Search for Error Messages in a log file</h2>

In this task, I must navigate to the ```/home/analyst/logs``` directory and report on the error messages in the ```server_logs.txt``` file. I’ll do this by using grep to search the file and output only the entries that are for errors.

1. Navigate to the ```/home/analyst/logs``` directory.
2. Use ```grep``` to filter the ```server_logs.txt``` file, and return all lines containing the text string ```error```.

Note: If I enter a command incorrectly and it fails to return to the command-line prompt, I can press CTRL+C to stop the process and force the shell to return to the command-line prompt.

Here I can see there are 6 error lines in the ```server_logs.txt``` file:

![image](https://github.com/n8som/Filter-with-grep/assets/110139109/fa857677-69cc-4efe-b2d0-110b581ccc34)

<h2>Task 2. Find files containing specific strings</h2>

In this task, I must navigate to the ```/home/analyst/reports/users``` directory and use the correct Linux commands and arguments to search for user data files that contain a specific string in their names.

1. Navigate to the ```/home/analyst/reports/users``` directory.

2. Using the pipe character (|), pipe the output of the ls command to the ```grep``` command to list only the files
containing the string ```Q1``` in their names.

Here, I can see 3 files that contain “Q1” in the ```/home/analyst/reports/users``` subdirectory:

![image](https://github.com/n8som/Filter-with-grep/assets/110139109/05a463ab-ccd0-43f5-8861-5039164d0e2f)

Note: Piping sends the standard output of one command to the standard input of another command for further processing. In the example, the output of the ```grep``` command is piped to the ls command and the output displayed in the shell.

3. List the files that contain the word ```access``` in their names.

Here, I can see 4 files in the ```/home/analyst/reports/users``` directory contain “access” in their names:

![image](https://github.com/n8som/Filter-with-grep/assets/110139109/8cd33f6b-48e4-45c2-b91d-6a032edffa11)

<h2>Task 3. Search more file contents</h2>

In this task, I must search for information contained in user files and report on users that were added and deleted from the system.

1. Display the files in the ```/home/analyst/reports/users``` directory.
2. Search the ```Q2_deleted_users.txt``` file for the username ```jhill```.

Here, I found the username ```jhill``` in the ```Q2_deleted_users.txt``` file:

![image](https://github.com/n8som/Filter-with-grep/assets/110139109/7f944711-a6f2-41f6-8255-dc4610ded88a)

3. Search the ```Q4_added_users.txt``` file to list the users who were added to the ```Human Resources``` department.

Note: For ```grep``` to interpret a string of two or more words correctly, I must enclose it in quotes (```"Human Resources"```).

Here I can see that 2 users were added to the HR department in quarter 4:

![image](https://github.com/n8som/Filter-with-grep/assets/110139109/a45cc209-89e2-4e7c-bcb0-a3952a13c4f8)

<h2>Conclusion</h2>

I now have practical experience in using ```grep``` to:

- search for specific information contained in files, and
- find files containing specific strings that were piped into ```grep```.

I'm well on my way to using fundamental tools in Linux to filter the information I need.

