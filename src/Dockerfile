FROM alpine 

RUN apk update
RUN apk add cmake git gcc
RUN git clone https://github.com/raspberrypi/pico-sdk
RUN cd pico-sdk
RUN export PICO_SDK_PATH=$PWD 
RUN echo $PICO_SDK_PATH
