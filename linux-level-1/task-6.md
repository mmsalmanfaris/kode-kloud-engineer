

    ssh into app sever2

    Use the find command to locate all files owned by john in the /home/usersdata directory, excluding directories.

     find /home/usersdata -type f -user john

            
            
          

    Use the find command combined with cp --parents to copy the files while preserving the directory structure.

     find /home/usersdata -type f -user john -exec cp --parents {} /blog \;

            
            
          

        /home/usersdata: Directory to search in.

        -type f: Locate files (excluding directories).

        -user john: Find files owned by the user john.

        -exec cp --parents {} /blog \;: For each file found, execute the cp --parents command to copy the file to the /blog directory, preserving the directory structure.
