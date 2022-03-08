# Speed Camera

## Purpose

- monitor the speed of people driving in front of my house
- take a piucture of each car and label it with its speed
- make a cool timelapse video and put it on youtube

## How

- Raspberry Pi Zero2 W
- Clone <https://github.com/pageauc/speed-camera.git> to the pi
- point the camera at the road
- add the starting of the scripts to the bottom of /etc/rc.local (above 'exit 0')
- calibrate and configure

## /etc/rc.local additions

```sh
cd /home/pi/speed-camera
python3 ./webserver.py &
python ./speed-cam.py &
```
