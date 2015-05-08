---
title: "processes"
bg: purple     #defined in _config.yml, can use html color like '#010101'
color: white #text color
fa-icon: gear
---

# Managing and killing processes

To list all processes on your system

`$ ps -aux`

To list all processes running as root

`$ ps -U root -u root u`

To list all processes owned by you

`$ ps x`

Searching processes by keyword

`$ ps -aux | grep '<keyword>'`

Listing it Tree style

`$ ps -aux --forest`

Killing a specific process

`$ sudo kill -9 <PID>`

Killing all processes except for kill and init

`$ sudo kill -9 -1` 