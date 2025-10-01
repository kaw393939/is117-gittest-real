# Question 10: What's the difference between absolute and relative paths? Give examples.

## Answer

**Absolute path** starts from the root directory (`/`) and gives the complete location. It always starts with `/`.

**Relative path** starts from your current location and describes where to go from there.

## Examples

**Absolute paths:**
```bash
/home/student/documents/file.txt
/usr/local/bin/python
```

**Relative paths:**
```bash
documents/file.txt          # file.txt in documents folder from here
../photos/vacation.jpg      # go up one level, then into photos
./script.sh                 # file in current directory
```

Absolute paths work from anywhere. Relative paths depend on where you are.