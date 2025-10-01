# Why is rm -rf dangerous?

The **rm -rf** command forcefully deletes files and directories without asking for confirmation. The -r flag means recursive (deletes folders and everything inside), and -f means force (no warnings).

If you accidentally run "rm -rf /" or "rm -rf *" in the wrong directory, you could delete your entire system or all your files instantly with no way to undo it. Always double-check before using this command.
