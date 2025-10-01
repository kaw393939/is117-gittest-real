# Question 9: How do you create a new directory? Provide the command and an example.

## Answer

Use the `mkdir` command (make directory) to create new folders.

## Examples

```bash
# Create a single directory
mkdir projects

# Create multiple directories
mkdir docs photos videos

# Create nested directories (parents too)
mkdir -p work/reports/2025
```

The `-p` flag is useful because it creates all parent directories if they don't exist.