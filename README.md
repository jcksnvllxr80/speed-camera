# Speed Camera

[![GitHub version](https://img.shields.io/github/release/jcksnvllxr80/speed-camera.svg)](lib-release)
[![GitHub download](https://img.shields.io/github/downloads/jcksnvllxr80/speed-camera/total.svg)](lib-release)
[![GitHub stars](https://img.shields.io/github/stars/jcksnvllxr80/speed-camera.svg)](lib-stars)
[![GitHub issues](https://img.shields.io/github/issues/jcksnvllxr80/speed-camera.svg)](lib-issues)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](lib-licence)

## Example Image

![alt text](./img/example_image.png "Example")

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
