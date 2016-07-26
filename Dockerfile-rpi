FROM sdhibit/rpi-raspbian

RUN apt-get update

RUN apt-get install -y git libncurses5-dev bison make gperf autoconf g++ g++-4.8 gcc gcc-4.8 python python-dev

RUN git clone https://github.com/cahirwpz/amigaos-cross-toolchain.git

# Add armv7l to supported architectures - as it works
RUN sed -e "s/\['i686'/\['armv7l', 'i686'/g" -i /amigaos-cross-toolchain/toolchain-m68k

# Build the toolchain - this will take a while
RUN /amiga-cross-toolchain/toolchain-m68k --prefix=/opt/toolchain build
