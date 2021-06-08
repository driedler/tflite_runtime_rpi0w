tflite_runtime Python wheel for Raspberry PI Zero W
=========================================================

Taken from:
https://www.tensorflow.org/lite/guide/build_cmake_pip


# Install Docker for WSL (if usng Windows)

See https://docs.docker.com/docker-for-windows/wsl/

# Build Python Wheel

```
# From Linux terminal (or WSL)
git clone --branch v2.5.0  https://github.com/tensorflow/tensorflow.git
cd tensorflow
sudo tensorflow/tools/ci_build/ci_build.sh PI-PYTHON38 \
  tensorflow/lite/tools/pip_package/build_pip_package_with_cmake.sh rpi0
```


