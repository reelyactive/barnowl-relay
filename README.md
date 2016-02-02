barnowl-relay
=============

A remote server relay for barnowl
---------------------------------

barnowl-relay augments a [barnowl](https://www.npmjs.com/package/barnowl) instance by relaying its real-time stream of events to a remote server, typically a [barnacles](https://www.npmjs.com/package/barnacles) instance.  Intended for command-line use.


Installation
------------

    npm install -g barnowl-relay

You may need to run the above as super-user (prefix the command with sudo).  Alternatively, use the Docker repository: reelyactive/barnowl-relay

    docker pull reelyactive/barnowl-relay


Examples
--------

### Relay a USB hub to www.hyperlocalcontext.com (default)

    barnowl-relay

### Relay a USB hub to www.hyperlocalcontext.com with console logging

    barnowl-relay -v

### Relay a USB hub to mybarnacles.io:8080

    barnowl-relay -h mybarnacles.io -p 8080

### Relay an IP hub to www.hyperlocalcontext.com

    barnowl-relay -u

### Relay multiple IP hubs to mybarnacles.io:8080 with console logging

    barnowl-relay -um -h mybarnacles.io -p 8080

### RTFM

    barnowl-relay --help


What's next?
------------

This is an active work in progress.  Expect regular changes and updates, as well as improved documentation! 


License
-------

MIT License

Copyright (c) 2016 reelyActive

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN 
THE SOFTWARE.
