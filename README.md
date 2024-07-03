# GStreamer Hello World

## Description
A Hello World application to demonstrate using GStreamer with cmake 3.22 
in a cross-platform configuration.

*This application has only been tested on Windows 10.

This demo can actually be written in a much simpler way, using GStreamer's 
textoverlay plugin for a similar effect. 
That way, Magick++ is not needed as a dependency.
This demo is created primarily to demonstrate a way to manipulate 
frames in a video or video stream.

## Dependencies
- pkg-config or Pkgconf
- GStreamer 1.0
- Magick++

## Build and Install

The following file's directory must be included 
in the shell's Path environment variable:

- pkgconf.exe or pkg-config

The following files' director(y/ies) must be included 
in the shell's PKG_CONFIG_PATH environment variable:

- gstreamer-1.0.pc
- gstreamer-sdp-1.0.pc
- gstreamer-app-1.0.pc
- gstreamer-video-1.0.pc

```powershell
mkdir build;
cd build;
cmake ..;
cmake --build . --config RelWithDebInfo;

cmake --install . #Run this line with administrative rights.
```

## Running

Navigate to your default installation directory (e.g., C:\Program Files),
the executable can be found installed at 
${INSTALL_DIR}/gstreamer_hello-world/bin/gstreamer_hello-world.exe