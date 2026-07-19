# SMART_DEVICE_MANAGEMENT_SYSTEM
# Smart Device Management System

## Overview
The **Smart Device Management System** is a Python Object-Oriented Programming (OOP) project that simulates the management of smart home devices. The system allows users to control different smart devices such as lights, security cameras, and temperature sensors through a simple command-line interface.

This project demonstrates the use of key OOP concepts including **Encapsulation, Inheritance, Polymorphism, and Method Overriding**.

---

## Features

- Display information about all smart devices.
- Turn all devices ON or OFF.
- Adjust the brightness of a smart light.
- Start and stop recording on a security camera.
- Read the current temperature from a temperature sensor.
- Interactive menu-driven interface.

---

## Technologies Used

- Python 3
- Object-Oriented Programming (OOP)

---

## OOP Concepts Demonstrated

### 1. Encapsulation
Private attributes are used to protect sensitive data.

```python
self.__device_id
self.__power
```

These attributes are accessed using getter and setter methods.

---

### 2. Inheritance

The base class **SmartDevice** is inherited by:

- SmartLight
- SecurityCamera
- TemperatureSensor

```python
class SmartLight(SmartDevice):
```

---

### 3. Method Overriding

Each subclass overrides the `display_info()` method to include device-specific information.

---

### 4. Polymorphism

The program calls the same method (`display_info()`) on different objects, and each object displays its own unique information.

---

## Class Structure

### SmartDevice
Base class that contains common attributes and methods.

**Attributes**
- name
- __device_id
- __power

**Methods**
- get_device_id()
- get_power()
- set_device_id()
- turn_on()
- turn_off()
- display_info()

---

### SmartLight

Additional Attribute:
- brightness

Methods:
- increase_brightness()
- decrease_brightness()
- display_info()

---

### SecurityCamera

Additional Attribute:
- recording

Methods:
- start_recording()
- stop_recording()
- display_info()

---

### TemperatureSensor

Additional Attribute:
- temperature

Methods:
- read_temperature()
- display_info()

---

## Program Menu

```
=== Smart Device Menu ===

1. Display Information
2. Turn Devices ON
3. Turn Devices OFF
4. Read Temperature
5. Adjust Brightness
6. Recording
7. Exit
```

---

## How to Run

1. Install Python 3 on your computer.

2. Save the program as:

```
smart_device_management.py
```

3. Open a terminal or command prompt.

4. Navigate to the project folder.

5. Run the program:

```bash
python smart_device_management.py
```

---

## Sample Output

```
=== Smart Device Menu ===

1. Display Information
2. Turn Devices ON
3. Turn Devices OFF
4. Read Temperature
5. Adjust Brightness
6. Recording
7. Exit

Choose an option: 2

Kitchen light is ON.
Outdoor Camera is ON.
Hall Sensor is ON.
```

---

## Project Structure

```
Smart-Device-Management-System/
│
├── smart_device_management.py
└── README.md
```

---

## Future Improvements

- Add more smart devices (Smart Fan, Smart Door Lock, Smart Thermostat).
- Save device information to a file or database.
- Add user authentication.
- Improve brightness limits (0–100%).
- Prevent recording when the camera is powered off.
- Display recording status as ON/OFF instead of True/False.
- Build a graphical user interface (GUI).

---

## Learning Outcomes

This project helps learners understand:

- Object-Oriented Programming in Python
- Encapsulation using private attributes
- Inheritance and code reuse
- Method overriding
- Polymorphism
- Menu-driven programming
- Class and object creation

---

## Author

**Name:** *AMOFA GIDEON*

**Course:** Object-Oriented Programming (OOP)

**Language:** Python

---

## License

This project is intended for educational purposes and may be modified or distributed for learning and academic use.
