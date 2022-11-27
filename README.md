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