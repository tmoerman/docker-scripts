# Danifold Mapper Container

Mapper is a GUI application, in order to run on Mac OS X:

- Run XQuartz 
- Start socat to expose local xquartz socket on a TCP port 
`socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\"` 
- Pass the display to container
`docker run -e DISPLAY=192.168.59.3:0 tmoerman/mapper`

(See: https://github.com/docker/docker/issues/8710)

