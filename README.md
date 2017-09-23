#Minimal (not) working example

This is a slightly modified version of the `minimal-qml` example from the official documentation.
The QT module `waylandcompositor` was added to the project file and a little dummy C++ snippet was added in `main.cpp` to access the QML object.

Running `qmake` fails with `Project ERROR: Library 'wayland-server' is not defined.`

Building with meson using
```
mkdir build
meson build/
ninja -C build/ all
```
successfully builds the compositor.
