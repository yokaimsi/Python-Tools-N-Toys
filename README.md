# Sting-Finder.py
This script searches for a specified string or word in large text files efficiently, using memory management and multithreading. It processes the file in chunks to avoid loading the entire file into memory, allowing you to search large files without exhausting system resources.

**How to Use:**
> Input File and Search String:\n
> Run the script and provide the path to the file you want to search.\n
> Enter the string you want to search for in the file.

**Optional: Save Results:**
> When prompted, you can choose whether to save all the matches to a file named `found.log` by typing `yes` or `no`.

**Memory Management:**
> The script limits memory usage by reading the file in manageable chunks (default 1MB).\n
> The `max_memory_usage` variable controls the total memory consumption (default is 2GB).

**Result:**
> The script will print the total number of occurrences of the search string.\n
> If enabled, all matched chunks will be saved in the found.log file.

**Key Functions:**
> `get_size()`: Estimates the memory usage of an object.\n
> `read_file_chunks()`: Reads the file in chunks.\n
> `search_in_chunk()`: Searches for the string in a single chunk.\n
> `search_in_file()`: Manages file processing, multithreading, and memory usage.\n

*The script will then search for "password123" in `largefile.txt`, show progress, and save all matches to found.log if you chose to do so.*
**Example Usage:**
```bash
Enter the path to the text file: /path/to/largefile.txt
Enter the string to search for: password123
Would you like to save all matches to 'found.log' file? (yes/no): yes```
