---
title: "permissions"
bg: blue     #defined in _config.yml, can use html color like '#010101'
color: white  #text color
style: left
fa-icon: lock
---

# File permissions

- To change the owner of a directory:
  
  `$ sudo chown -R newowner:newowner`

- To view actual files permissions

  `$ ls -l`
  
  - Example: `drwxr-xr-x`:
    - First letter is the file type:

      d          | b          | c            | p    | s      | \-
      :---------:|:----------:|:------------:|:----:|:------:|:-----------:
      directory  | block file | special file | pipe | socket | regular file

    - Second, third and fourth letters are the **user** permissions
    - Fifth, sixth and seventh letters are the **group** permissions
    - Eighth, ninth and tenth letters are the **others** permissions
    - Permissions
    
      r    | w     | x       | \-
      :---:|:-----:|:-------:|:------:
      read | write | execute | disable

- To change the files permissions:
  - Using letters: 
    - Which users:
    
      u    |   g   |    o   | a
      :---:|:-----:|:------:|:--:
      user | group | others | all
      
    - Operators:
    
      \+             |        \-         |                  =
      :-------------:|:-----------------:|:----------------------------------:
      add permission | remove permission | changes permissions to the inserted
      
    - Permissions: 
    
      r    | w     | x      
      :---:|:-----:|:------:
      read | write | execute

    - Example: `$ chmod a+w file` add **write** permission for **all** users
  - Using numbers
    - Permissions: 
    
      read | write | execute
      :---:|:-----:|:------:
        4  |   2   |    1
      
    - Example: `$ chmod 754 file` set permission to file:
    
       user                  |      group     |others
      :---------------------:|:--------------:|:------:
       7                     |       5        |  4
      read + write + execute | read + execute | read
