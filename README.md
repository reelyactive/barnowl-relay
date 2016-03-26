barnowl-relay
=============

A remote server relay for barnowl
---------------------------------

barnowl-relay is a simple command-line tool that relays data from radio-sensors to a remote server.  A typical use case is to connect a [reelyActive starter kit](http://shop.reelyactive.com/collections/starter-kits) to the cloud via your PC or a Raspberry Pi.

Technically, barnowl-relay is simply an augmented [barnowl](https://www.npmjs.com/package/barnowl) instance, configured to relay its real-time stream of events to a remote server, typically a [barnacles](https://www.npmjs.com/package/barnacles) instance.


Installation
------------

### Windows and Mac

    npm install -g barnowl-relay

### Linux

    sudo npm install -g barnowl-relay

### Docker

    docker pull reelyactive/barnowl-relay


Usage with USB Hub
------------------

For use with a [minimal starter kit](http://shop.reelyactive.com/products/starterkit-min) connected to the computer.

### Relay to www.hyperlocalcontext.com (default)

    barnowl-relay -s

### Relay to cloud.reelyactive.com

    barnowl-relay -s -h cloud.reelyactive.com


Usage with IP Hub
-----------------

For use with a [BLE starter kit](http://shop.reelyactive.com/products/starterkit-ble) or equivalent which is sending UDP packets to the computer.

### Relay to www.hyperlocalcontext.com (default)

    barnowl-relay -um

### Relay to cloud.reelyactive.com

    barnowl-relay -um -h cloud.reelyactive.com


Advanced Parameters
-------------------

### Verbose output

By default, barnowl-relay will only log errors to the console.  To log all relayed messages, run as follows:

    barnowl-relay -v

### Relay to a specific host

By default, barnowl-relay will POST to www.hyperlocalcontext.com.  To instead use mybarnacles.io, for instance, run as follows:

    barnowl-relay -h mybarnacles.io

### Relay to a specific port

By default, barnowl-relay will POST to port 80.  To instead use port 8080, for instance, run as follows:

    barnowl-relay -p 8080

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
