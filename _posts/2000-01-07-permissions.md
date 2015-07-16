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


- To change the files permissions:
  - Using letters: 
    - Which users:
      - u: user
      - g: group
      - o: others
      - a: all
    - Operators:
      - \+ (add permission)
      - \- (remove permission)
      - = (changes permissions to the informed)
    - Permissions: 
      - r: read
      - w: write
      - x: execute
    - Example: `$ chmod a+w file` add write permission for all users
  - Using numbers
    - Permissions: 
      - 4 (read)
      - 2 (write)
      - 1 (execute)
    - Example: `$ chmod 754 file` set permission to file:
      - user = 7 (read + write + execute)
      - group = 5 (read + execute)
      - others = 4 (read)
