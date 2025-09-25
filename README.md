# gtkmm4-gesture-ai-sample-test
This small sample C++ code which try show possible using gtkmm4  mouse gesture recognition with AI this code is possible to build and run on Debian13 or on Windows in MSYS2 enviroment.

# Building on Windows
# Install MSYS2
Download and run the msys2 installer from http://msys2.github.io/ I’ve only tested with the 64bit version. Make sure that the path you select for installation doesn’t contain any spaces.

# Start MSYS console
Launch the Start Menu item “MSYS2 mingw 64 bit” you should be greeted with a console window. All steps below refer to what you should type into that window.

# Install updates
Type:

pacman -Syu
if it tells you to close restart msys, close the console window and start it again. Then run pacman -Syu again.

# Install dependencies
Type/paste

pacman -S \
mingw-w64-x86_64-gcc \
mingw-w64-x86_64-pkgconf \
mingw-w64-x86_64-gtkmm4 \
zip \
unzip \
git \
--needed

When prompted, just hit return. Sit back and wait for it to install what’s almost a complete linux environment.

Before continuing you may change to another directory. It easiest to type cd followed by a space and drop the folder you want to change to on the window.

# To clone gtkmm4-gesture-ai-sample-test run:

git clone https://github.com/Peta-T/gtkmm4-gesture-ai-sample-test
cd gtkmm4-gesture-ai-sample-test
To build it run on command line:
 g++ -std=c++20 main.cc `pkg-config --cflags --libs gtkmm-4.0 ` -o app -g

# To run app type on command line:
./app


