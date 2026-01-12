---
layout: page
title: Multi-Client Chat Server
description: 
img: assets/img/multi_client_chat_server.png
importance: 2
category: 
---

<strong>Github Source Files</strong>: [https://github.com/CapeGenius/Multi-Client-Chat-Server](https://github.com/CapeGenius/Multi-Client-Chat-Server)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/multi_client_chat_server.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <em>Screenshot of Linux Bash commands to start client</em>
</div>

I worked on a team of three to develop a multithreaded chat application in C for my Software Systems course. The system is designed to initialize a server, accept and manage multiple concurrent client connections, and support real-time message exchange between connected users. We implemented a custom length-prefixed messaging protocol to ensure reliable communication over TCP, used pthreads to manage concurrency on both the server and client sides, and incorporated thread-safe message logging to track activity across active connections.




