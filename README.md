[![Docker Stars](https://img.shields.io/docker/stars/frolvlad/alpine-gxx.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-gxx/)
[![Docker Pulls](https://img.shields.io/docker/pulls/frolvlad/alpine-gxx.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-gxx/)


C/C++ (GCC) Docker image
========================

This image is based on Alpine Linux image, which is only a 5MB image, and contains
[C/C++ compilers](https://gcc.gnu.org/) (gcc/g++ packages).

Download size of this image is only:

[![](https://images.microbadger.com/badges/image/frolvlad/alpine-gxx.svg)](http://microbadger.com/images/frolvlad/alpine-gxx "Get your own image badge on microbadger.com")


Usage Example
-------------

```bash
$ echo -e '#include <iostream>\nint main() { std::cout << "Hello World\\n"; }' > qq.cpp
$ docker run --rm -v `pwd`:/tmp frolvlad/alpine-gxx c++ --static /tmp/qq.cpp -o /tmp/qq
```

Once you have run these commands you will have `qq` executable in your current directory and if you
execute it, you will get printed 'Hello World'!
