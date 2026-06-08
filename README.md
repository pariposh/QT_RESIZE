QT_RESIZE

A professional Qt GUI auto-resizing utility designed for QWidget-based desktop applications.
The tool scans Qt Designer .ui files, extracts widget geometry information, and automatically generates responsive resize handling code for dynamic GUI scaling.

Ideal for modernizing fixed-resolution Qt applications without redesigning the entire interface using layouts.

Overview

QT_RESIZE simplifies the process of making legacy Qt GUIs responsive by automatically generating geometry-based scaling code from existing .ui files.

The tool analyzes widgets defined inside mainwindow.ui (or any Qt Designer UI file) and produces ready-to-use resize logic that dynamically scales and repositions widgets during window resizing.

This is especially useful for:

Legacy Qt projects using absolute positioning
Embedded Linux / HMI applications
Jetson-based Qt applications
FPGA/Control system GUIs
Rapid migration of fixed-size interfaces to scalable displays
Features
Automatic parsing of Qt .ui files
Extracts:
Widget object names
Geometry information
Parent-child hierarchy
Generates:
QMap<QWidget*, QRect> initialization
Original geometry capture code
Dynamic resizeEvent() scaling implementation
Supports QWidget-based applications
Reduces manual resize coding effort
Helps maintain proportional GUI scaling across resolutions
Works well with Qt Designer generated interfaces
Generated Output

The generated code includes:

Initial widget geometry storage
Automatic resize scaling logic
Geometry restoration calculations
Proportional widget repositioning and resizing

Use Cases
Qt Widgets applications
Industrial HMIs
Embedded GUI systems
Jetson/ARM Linux interfaces
Control systems
Monitoring dashboards
Rapid UI modernization projects

Why QT_RESIZE?

Many legacy Qt applications were developed using fixed widget geometries instead of layouts.
Rebuilding such applications with proper layouts can be time-consuming and risky.

QT_RESIZE provides a fast and practical solution by automatically generating responsive scaling logic while preserving the original UI design.
