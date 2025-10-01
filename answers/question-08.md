# Question 8: What does `ls -la` show you that `ls` alone does not?

## Answer

`ls -la` shows much more information than plain `ls`:

- **`-l`** (long format): Shows permissions, owner, size, and modification date
- **`-a`** (all files): Shows hidden files (files starting with `.`)

## Comparison

```bash
$ ls
file1.txt  file2.txt

$ ls -la
total 24
drwxr-xr-x 2 student student 4096 Oct  1 10:00 .
drwxr-xr-x 5 student student 4096 Oct  1 09:00 ..
-rw-r--r-- 1 student student  256 Oct  1 10:00 .hidden
-rw-r--r-- 1 student student  512 Oct  1 10:00 file1.txt
-rw-r--r-- 1 student student  128 Oct  1 10:00 file2.txt
```

Notice it shows `.hidden` file and detailed information!