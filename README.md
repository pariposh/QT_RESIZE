# QT_RESIZE
A Qt GUI auto-resizing helper tool that extracts widget geometries from .ui files and generates dynamic scaling code for responsive QWidget-based applications.

Automatic Qt GUI resize code generator for QWidget-based applications.

Features
Parses Qt .ui files automatically
Extracts all widget object names
Generates:
QMap<QWidget*, QRect>
initial geometry capture code
resizeEvent() scaling implementation
Helps convert fixed-size Qt GUIs into responsive scalable interfaces
Useful for legacy Qt Designer projects without layouts
