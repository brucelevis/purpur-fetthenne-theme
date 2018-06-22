
# Building

## Get Dear Imgui

git clone https://github.com/ocornut/imgui

## Get GLFW

### Install Libraries

sudo apt install libglfw3 libglfw3-dev

### Build It

git clone git@github.com:glfw/glfw.git
http://www.glfw.org/docs/latest/compile.html

## Update CMakeLists File

Update the paths in the CMakeLists file for gl3w and imgui. GL3W is included with Dear Imgui.

## Get Roboto Font

$ mkdir robot
$ cd robot
$ wget https://github.com/google/roboto/releases/download/v2.138/roboto-android.zip
$ unzup roboto-android.zip

## Run from Project Root

You must run from the project root so that the code can find the Roboto Font. You could
also modify the path to the font in the code.

$ mkdir build
$ cd build
$ cmake -GNinja ..
$ ninja
$ cd ..
$ ./build/imgui-theme