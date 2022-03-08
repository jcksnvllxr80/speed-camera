# Speed Camera

## Purpose

To monitor the speed of people driving in front of my house.

## How

- Raspberry Pi Zero2 W
- Clone <https://github.com/pageauc/speed-camera.git> to the pi
- point the camera at the road
- add the start scripts to the bottom of /etc/rc.local (above 'exit 0')

## /etc/rc.local additions

```sh
cd /home/pi/speed-camera
python3 ./webserver.py &
python ./speed-cam.py &
```
