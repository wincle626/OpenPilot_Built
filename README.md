# OpenPilot_Built
This is a repo that with modified OpenPilot Makefile and successfully built the source code.

You need to modify the make/tool.mk files to the updated link of all required tools, such as gtest, doxygen and uncrustify, with right version. Or you can comment the script lines for downloading from existing link and download the pakcage by yourself. I suggest the second way. Besides, you might need to install flex and bison through apt-get as well for doxygen. 

Some prerequiresites such as OpenGL, SDL, etc.

Installing OpenGL following this link: https://en.wikibooks.org/wiki/OpenGL_Programming/Installation/Linux

sudo apt-get install build-essential libgl1-mesa-dev
sudo apt-get install libglew-dev libsdl2-dev libsdl2-image-dev libglm-dev libfreetype6-dev

Install SDL following this link: http://www.damnsmalllinux.org/f/topic-3-9-15913-0.html

sudo apt-get install libsdl-dev libsdl-1.0.0-dev

As we only need the ground station control (gcs), just run:

make all_sdk_install && make gcs
