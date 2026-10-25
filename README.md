# IoT-Based Traffic Management System

An IoT-based traffic management project designed to monitor vehicle proximity and demonstrate traffic-light control using sensor data. The project explores the integration of embedded hardware, IoT connectivity, cloud services, and web-based traffic monitoring to support more adaptive urban traffic management.

## Overview

Traditional traffic signals often rely on fixed timing, which may not respond effectively to changing traffic conditions. This project explores how Internet of Things (IoT) technologies can help improve traffic monitoring and signal control by collecting sensor data and using it to determine traffic-light states.

The prototype uses an ultrasonic sensor to measure distance, a Raspberry Pi-based setup for processing, and LEDs to represent traffic signals. The project also explores connecting device telemetry to Microsoft Azure for cloud-based monitoring and analysis.

## Project Purpose

This project explores the application of embedded systems, IoT sensing, traffic-light control, and cloud computing to an urban mobility problem. It serves as a prototype for investigating how connected devices and sensor data can support more responsive traffic management.

## Objectives

- Demonstrate vehicle-proximity detection using an ultrasonic sensor.
- Control traffic-light indicators based on measured distance.
- Explore IoT communication between embedded devices and cloud services.
- Investigate cloud-based storage, real-time data processing, and traffic visualization.
- Explore how sensor-driven traffic control could contribute to more efficient urban mobility.

## Technologies and Components

### Hardware

- Raspberry Pi
- HC-SR04 ultrasonic distance sensor
- LEDs for traffic-light simulation
- Resistors
- Breadboard and connecting wires

### Software and Platforms

- Python / MicroPython-style GPIO programming
- Wokwi online hardware simulator
- Microsoft Azure IoT Hub
- Azure Functions
- Azure Stream Analytics
- Azure Blob Storage
- Azure Web Apps
- Azure Cosmos DB (proposed data-storage option)

## System Architecture

The proposed system consists of the following stages:

1. **Sensing:** The ultrasonic sensor measures the distance to a nearby object, representing vehicle proximity.
2. **Processing:** The device reads the sensor measurements and applies threshold-based logic.
3. **Signal control:** LEDs represent traffic-light states based on the measured distance.
4. **IoT connectivity:** Sensor telemetry can be transmitted to Azure IoT Hub for cloud integration.
5. **Cloud processing and visualization:** Azure services are considered for processing traffic data, storing historical information, and displaying traffic status through a web-based dashboard.

## Traffic-Light Control Logic

The prototype uses distance thresholds to demonstrate sensor-driven signal control.

| Measured distance | Demonstrated signal state |
|---|---|
| Less than 10 cm | Yellow LED |
| 10 cm to less than 20 cm | Red LED |
| 20 cm or greater | Green LED |

The program measures distance repeatedly and updates the LED outputs according to these thresholds. These values are intended for demonstration and are not suitable as-is for real-world traffic signal deployment.

## Simulation

The project includes Wokwi simulations for the sensor-driven traffic management prototype.

- [Traffic Management Simulation — Wokwi](https://wokwi.com/projects/378915192728578049)
- [Traffic Management Simulation initializing Azure IoT Hub Client — Wokwi](https://wokwi.com/projects/380209624943953921)

## Azure Cloud Integration

The project explores using Microsoft Azure to extend the prototype beyond local sensor processing.

- **Azure IoT Hub:** Communication between the device and the cloud.
- **Azure Stream Analytics:** Processing incoming telemetry and identifying traffic patterns.
- **Azure Functions:** Executing event-triggered processing tasks.
- **Azure Blob Storage:** Storing traffic images and video, where camera integration is implemented.
- **Azure Web Apps:** Hosting a dashboard for viewing traffic information.
- **Azure Cosmos DB:** Storing structured traffic events and historical data.

These services form the proposed cloud architecture; their availability and integration depend on the corresponding deployment and configuration.

## Project Development

The project was developed in phases:

1. Identifying traffic congestion, safety, and environmental challenges.
2. Designing an IoT-based architecture using Raspberry Pi and sensors.
3. Developing sensor-based traffic-light control logic.
4. Exploring communication with Azure IoT Hub and cloud-based processing.
5. Building and testing hardware or simulated prototypes.


