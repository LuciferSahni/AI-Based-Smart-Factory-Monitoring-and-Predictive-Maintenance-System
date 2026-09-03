# AI-Based Smart Factory Monitoring and Predictive Maintenance System

An Industrial IoT and AI-based predictive maintenance system designed to monitor industrial motor health in real time using multiple sensors, wireless communication, and machine learning-based anomaly detection.

## Overview

Industrial machines can experience failures due to abnormal vibration, temperature, voltage, current, or rotational speed. This project aims to continuously monitor these parameters and identify abnormal operating conditions before they lead to equipment failure.

The system combines embedded hardware, IoT communication, data analytics, and machine learning to provide real-time equipment health monitoring and predictive maintenance insights.

## System Architecture

Industrial Motor
        ↓
     Sensors
        ↓
      STM32
        ↓
      ESP32
        ↓
      Wi-Fi
        ↓
 MQTT / Firebase
        ↓
 Python Backend
        ↓
Real-Time Dashboard
        ↓
Equipment Health & Maintenance Alerts

## Parameters Monitored

- Vibration
- Temperature
- Voltage
- Current
- RPM (Rotational Speed)

## Hardware Components

- STM32 Microcontroller
- ESP32 Development Board
- MPU6050 – Vibration / Motion sensing
- DS18B20 – Temperature sensing
- Voltage Sensor
- Current Sensor
- RPM / Proximity Sensor
- Industrial Motor

## Software & Technologies

- Embedded C/C++
- STM32
- ESP32
- Python
- NumPy
- Pandas
- Scikit-learn
- MQTT
- Firebase
- Data Visualization
- Real-Time Monitoring Dashboard

## Working

1. Sensors continuously collect operating parameters from the industrial motor.
2. STM32 acquires and processes the sensor data.
3. The processed data is transferred to the ESP32.
4. ESP32 transmits the equipment telemetry through Wi-Fi.
5. MQTT/Firebase is used for communication and data transmission.
6. A Python-based backend processes and analyzes the incoming telemetry.
7. Machine learning techniques are applied to identify abnormal operating patterns.
8. The dashboard displays real-time equipment parameters and machine health information.
9. Abnormal conditions can be used to generate maintenance alerts and support proactive maintenance decisions.

## Machine Learning

The collected sensor data is analyzed to identify patterns associated with abnormal machine operation.

The ML pipeline includes:

- Data preprocessing
- Feature extraction
- Feature engineering
- Anomaly detection
- Equipment health analysis
- Maintenance insight generation

## Dashboard

The real-time monitoring dashboard is designed to display:

- Current sensor readings
- Vibration levels
- Temperature
- Voltage
- Current
- RPM
- Equipment health status
- Historical readings
- Abnormal-condition alerts

## Project Objectives

- Enable real-time industrial equipment monitoring
- Detect abnormal machine operating conditions
- Apply AI/ML for predictive maintenance
- Reduce unexpected equipment downtime
- Provide data-driven maintenance insights
- Demonstrate an end-to-end Industrial IoT architecture

## Future Scope

- Edge AI deployment directly on ESP32
- Remaining Useful Life (RUL) prediction
- Automated fault classification
- Cloud-based monitoring
- Digital twin integration
- Automated maintenance scheduling

## Disclaimer

This project is an independent implementation inspired by Industrial IoT predictive-maintenance architectures. Hardware configuration, software implementation, datasets, and results may vary depending on the implementation.
