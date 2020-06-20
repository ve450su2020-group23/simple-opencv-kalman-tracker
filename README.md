# simple-opencv-kalman-tracker: update
This repo has converted the original codes to accommodate OpenCV 4.3.0 with a command line parser.

## Requirements
- OpenCV 4.3.0 with **the following packages:**
  - `libgtk` or Qt. (GUI support)
  - `libavcodec-dev libavformat-dev libswscale-dev libv4l-dev` (Read video file from disk support)

Compiling OpenCV 4.3.0 with Qt GUI and FFmpeg support:
```bash
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr/local -DWITH_QT=on -DCMAKE_PREFIX_PATH=<path/to/your/Qt/lib> -DWITH_FFMPEG=ON ..
make 
sudo make install
```

## Usage
To compile this code, `cd` to the root of this repo and type
```bash
mkdir build && cd build
cmake ..
make
```

To run this code, type
```bash
./simple-opencv-kalman-tracker --video=/path/to/your/video/file
```

**Note.** `./simple-opencv-kalman-tracker -h` would print help messages for this executable.

***BELOW ARE THE ORIGINAL README...***

# simple-opencv-kalman-tracker
A simple Ball Tracker made using OpenCV to demonstrate the use of the Kalman Filter in Computer Vision

You can find the full tutorial on [Robot-home website](http://www.robot-home.it/blog/en/software/ball-tracker-con-filtro-di-kalman/)

Watch the demo working on YouTube: https://www.youtube.com/watch?v=sG-h5ONsj9s
