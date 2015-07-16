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
    - Operators:
      - \+ (add permission)
      - \- (remove permission)
      - = (changes permissions to the informed)
    - Which users:
      - u: user
      - g: group
      - o: others
      - a: all
    - Permissions: 
      - r: read
      - w: write
      - x: execute
    - Example: `$ chmod a+w file` add write permission for all users
