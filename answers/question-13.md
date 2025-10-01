# Question 13: Why is the `rm -rf` command dangerous? How can you be safer?

## Answer

`rm -rf` is dangerous because:
- **`rm`** = remove (delete permanently)
- **`-r`** = recursive (delete directories and everything inside)
- **`-f`** = force (don't ask for confirmation, ignore warnings)

It can delete entire directories without asking, and there's NO undo or trash bin in Linux!

## Safer Alternatives

```bash
# Use -i for interactive (asks before each deletion)
rm -i file.txt

# Use -r without -f (still prompts for dangerous operations)
rm -r folder/

# Always double-check what you're deleting
ls folder/      # Check contents first
rm -r folder/   # Then delete
```

**Never run `rm -rf /` or `rm -rf *` without being absolutely sure!**