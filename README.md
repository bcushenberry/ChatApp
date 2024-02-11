# Overview

What I want to do with this project is to make a simple chat app that is able to send files between two computers, either via a local network or peer-to-peer. (I'm leaning toward peer-to-peer.)

I initially started with a client/server setup, but only to get a feel for how such things work. In this case, you can open client.py in one terminal and server.py in another, and whatever you send in the client.py terminal will also show up in the server.py terminal. This is essentially a proof of concept.

I will likely change this up to go with peer-to-peer. I would like to add a GUI to the program. Also, and perhaps most importantly, you can't currently send files, only messages. There is still work to be done.

[Demonstration Video (Pending)]()

# Network Communication

Currently, this uses a client/server architecture, though I may rework it into peer-to-peer.

TCP is used over UDP because we don't want lost packets and the order in which the packets are sent/arrive is important. Currently, port 55555 is used, but that could change.

# Development Environment

The development of this software was done using VS Code and the Python, Pylance, Python Debugger plugins.

Currently, only the "socket" library is used, but in the final version I think "threading" might also be used. I found a few custom libraries as well that seem quite good, but they might be too complicated for this project (and they might do too much of the heavy lifting).

# Useful Websites

Youtube is a great resource for tutorials. Most of the time I've spent so far on this project is learning about how networking works, how sockets work, etc. One particularly helpful tutorial is the Python Sockets Simply Explained video linked below. Also, I've not tried the peer-to-peer architecture just yet, but I found what looks to be a useful tutorial on LinkedIn.

* [Python Sockets Simply Explained (Youtube)](https://www.youtube.com/watch?v=YwWfKitB8aA)
* [Implementing Peer-to-Peer Data Exchange in Python (LinkedIn)](https://www.linkedin.com/pulse/implementing-peer-to-peer-data-exchange-inpython-luis-soares-m-sc-/)

# Future Work

There is a lot of work to still be done.
* Rework the architecture to peer-to-peer
* Add file-sharing functionality
* Add GUI