# Finding Files

### What I learned
How to locate files, directories, and binary paths in Linux.

### Commands:
- `locate <filename>`: Quickly searches for files using the pre-built locate database.
- `sudo updatedb`: Updates the database index used by the `locate` command.
- `find <directory> -name "<filename>"`: Searches for a file in real-time within the specified directory.
- `find <directory> -name "*<keyword>*"`: Searches for files containing the keyword using wildcards (`*`).
- `find / -name "<filename>"`: Searches the entire filesystem starting from the root directory (`/`).
- `whereis <command>`: Displays the binary, source, and manual page locations for a command.
- `which <command>`: Shows the absolute path of the executable found in the system `$PATH`.