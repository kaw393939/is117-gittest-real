# Question 15: How would you view the last 20 lines of a log file?

## Answer

Use the `tail` command with the `-n` option to specify how many lines you want to see.

## Command

```bash
tail -n 20 logfile.log
```

Or shorter version:
```bash
tail -20 logfile.log
```

## Bonus: Follow Live Updates

To watch a log file in real-time as new lines are added:

```bash
tail -f logfile.log
```

This is super useful for monitoring application logs or system logs. Press `Ctrl+C` to stop following.