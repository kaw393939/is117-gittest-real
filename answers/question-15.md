# How do you view last 20 lines of a file?

Use the **tail** command with the -n flag: tail -n 20 filename.txt

This displays only the last 20 lines of the file, which is useful for large files or log files where you only care about recent entries.

You can also use **tail -f filename.txt** to follow a file in real-time, showing new lines as they're added (great for monitoring logs).
