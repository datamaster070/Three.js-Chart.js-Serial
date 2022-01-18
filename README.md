# [WebSerialChart](https://infomorph-inc.github.io/WebSerialChart/index.html)
Web Serial, Chart.js, Three.js sample

## Overview
This software gets the USB Serial data and shows the real-time chart on the web browser.
This code is a sample code for checking implementation and the work of IMU via USB serial.

## Screenshot
![screenshot](images/WebSerialChart.png)

## What is this
We use [Web Serial API](https://wicg.github.io/serial/) to get serial data on the web, [Chart.js](https://www.chartjs.org/) and [chartjs-plugin-streaming](https://nagix.github.io/chartjs-plugin-streaming/) to show the chart.

### USB Serial data format
We tried to measure IMU data output from [Atom Matrix](https://docs.m5stack.com/#/en/core/atom_matrix). The original code is [here](https://github.com/m5stack/M5Atom/edit/master/examples/Basics/MPU6886/MPU6886.ino). Please change its serial output format as below.

The USB Serial format should be Euler(XYZ-order,"%f,%f,%f¥n") or Quaternion(x,y,z,w order, "%f,%f,%f,%f¥n").

## Try to use
1. [Check this live demo page](https://infomorph-inc.github.io/WebSerialChart/index.html).
2. Click the "Open Serial Port" button to open the serial port.
3. Rotate the airplane by mouse if you want to change the view angle.
4. Click the "Pause Chart" button to stop and resume the chart flow.

## License
* Our software is licensed under GPLv2.
* We use Three.js ver.1.0.8.
* Included aircraft 3D model "b789.gib" is derived from [Flightradar24 3D models](https://github.com/Flightradar24/fr24-3d-models) which is licensed under GPLv2.
