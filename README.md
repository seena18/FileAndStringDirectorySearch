# FileAndStringDirectorySearch
Shell program which can recursively search for different files with either the name of the file or a string contained within the file. Returns the path of the file.

Each search deploys a child process to search, so the user can run multiple searches at once. 
Child process will interrupt the parent process with results once it has completed its search.

**Program uses four following commands:**

**find:**
    -"find" followed by the name of a file or a string. Will return said file or any file containing the string). Ex.(find program.c) (find "string")
    - the arguement -f: allows you to specify what type of file you are looking for when searching with a string. 
      Ex.(find "string" -f:c) this will search for C extension files
    - the arguement -s will search for files within all branching folders that extend beyond the current directory
    - arguements -f: and -s can be used together
    
**list:**
    -lists all the running child processes
    
**kill:**
    -ends any child process with the associated serial key provided in the list command. Ex.(kill 1)
    
**quit or q**
    -ends all processes 
    
