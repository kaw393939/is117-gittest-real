# Question 14: What does the `cat` command do? Provide an example use case.

## Answer

`cat` displays the entire contents of a file(s) in the terminal. The name comes from "concatenate" because it can join multiple files together.

## Use Cases

**View a file:**
```bash
cat notes.txt
```

**View multiple files:**
```bash
cat file1.txt file2.txt
```

**Create a new file with content:**
```bash
cat > newfile.txt
Type some content here
Press Ctrl+D to save
```

**Combine files:**
```bash
cat part1.txt part2.txt > combined.txt
```

Best for small files. For large files, use `less` instead.