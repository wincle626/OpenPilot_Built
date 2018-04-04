# OpenPilot_Built
This is a repo that with modified OpenPilot Makefile and successfully built the source code.

You need to modify the make/tool.mk files to the updated link of all required tools, such as gtest, doxygen and uncrustify, with right version. Or you can comment the script lines for downloading from existing link and download the pakcage by yourself. I suggest the second way. Besides, you might need to install flex and bison through apt-get as well for doxygen. 
