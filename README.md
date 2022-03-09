# Speed Camera

[![GitHub version](https://img.shields.io/github/release/jcksnvllxr80/speed-camera.svg)](lib-release)
[![GitHub download](https://img.shields.io/github/downloads/jcksnvllxr80/speed-camera/total.svg)](lib-release)
[![GitHub stars](https://img.shields.io/github/stars/jcksnvllxr80/speed-camera.svg)](lib-stars)
[![GitHub issues](https://img.shields.io/github/issues/jcksnvllxr80/speed-camera.svg)](lib-issues)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](lib-licence)

## Purpose

- monitor the speed of people driving in front of my house :truck:
- take a picture of each car and label it with its speed :camera:
- make a cool time-lapse video and put it on youtube :tv: <https://youtu.be/GM9vSAUtNBc>
- make cool graphs to analyze the data :bar_chart: :chart_with_downwards_trend: (Charts/Graphs Below!)

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

## Example Image

![alt text](./img/example_image.jpg "Example")

## Charts / Graphs

### Average Speed vs. Day

![alt text](./graphs/AverageSpeed_vs_Day.png "Average Speed vs. Day")

### Car Count vs. Hour

![alt text](./graphs/car_count_by_hour.png "Car Count vs. Hour")

### Frequency of Speed

![alt text](./graphs/frequency_of_speed.png "Frequency of Speed")

### Speed's Normal Distribution

![alt text](./graphs/Speed_normal_distribution.png "Speed's Normal Distribution")

### Average Speed vs. Direction (L2R or R2L)

![alt text](./graphs/ave_speed_by_direction.png "Average Speed vs. Direction (L2R or R2L)")

### Average Speed vs. Hour

![alt text](./graphs/AverageSpeed_vs_Hour.png "Average Speed vs. Hour")

### Car Count vs. Day

![alt text](./graphs/car_count_by_day.png "Car Count vs. Day")
