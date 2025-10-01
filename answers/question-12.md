# Question 12: Explain the difference between `cp` and `mv` commands.

## Answer

**`cp` (copy)** creates a duplicate of the file/directory. The original stays in place.

**`mv` (move)** relocates the file/directory OR renames it. The original is gone from its old location.

## Examples

```bash
# cp - makes a copy, original remains
cp report.txt backup.txt
# Now you have both report.txt AND backup.txt

# mv - moves or renames, original gone
mv report.txt documents/
# Now report.txt is ONLY in documents/

mv oldname.txt newname.txt
# File is renamed, oldname.txt no longer exists
```

Key difference: `cp` = keep original, `mv` = remove original.