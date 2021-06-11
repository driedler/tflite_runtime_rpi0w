tflite_runtime Python wheel for Raspberry PI Zero W
=========================================================

Taken from:
https://www.tensorflow.org/lite/guide/build_cmake_pip


# Install Docker for WSL (if using Windows)

See https://docs.docker.com/docker-for-windows/wsl/

# Build Python Wheel

```
# From Linux terminal (or WSL)


git clone --branch v2.5.0  https://github.com/tensorflow/tensorflow.git
cd tensorflow
sudo ./tensorflow/tools/ci_build/ci_build.sh PI-PYTHON37 tensorflow/lite/tools/pip_package/build_pip_package_with_cmake.sh rpi0
```

After the above commands run, the built wheel should be found at (in your Linux or WSL terminal):
```
./tensorflow/lite/tools/pip_package/gen/tflite_pip/python3.7/dist/
```

# Install 

To install, issue the following command on your RPI

```
sudo pip3 install https://github.com/driedler/tflite_runtime_rpi0w/raw/master/tflite_runtime-2.5.0-cp37-cp37m-linux_armv6l.whl
```
