[![Build Status](https://travis-ci.org/nidium/Nidium.svg?branch=master)](https://travis-ci.org/nidium/Nidium)

# nidium

nidium is an ongoing effort for a general purpose rendering engine to create apps, games on both Desktop and mobile and also serverside applications.

nidium helps you create graphical softwares with JavaScript. It's **not** NodeJS, QT, Chromium, or a WebKit derivate. It has been designed from scratch and has a small codebase written in C++.

It leverages the combination of **Skia** Graphics from Google, and Mozilla's JavaScript Engine (**SpiderMonkey**) and many more awesome librairies. 

nidium also ships with its own layout engine.

It supports various common well known API such as :

* **WebGL**
* **Canvas 2D Context**
* **WebSocket** (client & server)
* **Module loading** (require())

And some other non standard :

* **UDP/TCP Socket**
* **Files**
* **Threaded Audio**
* **videos** (libav integration)
* **Fragment shader on 2d canvas**
* **HTTP** (Client & server)
* **Local storage**

It can seemlessly runs various library like Three.JS, PixiJS, Phaser and probably a lot more without much modification.

## Building nidium

To build nidium you need at least 5GB of disk space. A build from scratch will take between 30min to 1H30, depending of the speed of your computer.

```
$ apt-get install libpci-dev python2.7 git make patch clang pkg-config libgtk2.0-dev libgtk-3-dev mesa-common-dev libglu1-mesa-dev yasm libasound2 libasound2-dev libbz2-1.0

$ git clone https://github.com/nidium/NidiumTools.git
$ git clone --recursive https://github.com/nidium/Nidium.git
$ export PYTHONPATH=$(pwd)/NidiumTools/src
$ cd Nidium
$ ./configure_frontend
$ ./bin/nidium
```

## License

Copyright 2016 Nidium Inc. All rights reserved.
Use of this source code is governed by a MIT license that can be found in the LICENSE file.
