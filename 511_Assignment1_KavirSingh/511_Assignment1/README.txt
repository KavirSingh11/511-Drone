In order to compile using the OpenGL libraries, download the Freeglut files
In some cases it is necessary to go into a computers program files and go to Common Files
and under Common Files make a new MSVC directory and in that directory make a freeglut file, in this directory add the include and lib from the freeglut download
folders in the freeglut download

To link freeglut to the project

1. Open properties from right clicking on the solution folder
2. Click on VC++ Directories
3. Under Include Directories go to the file destination for the include folder that was saved in your program files and add it
4. Under Libary Directories go to the file destination for the lib folder that was saved in your program files and add it
5. Under the Linker tab, go to Input and under additional dependencies add freeglut.lib and opengl32.lib. 
6. In some cases (including mine) it was necessary to actually include the freeglut.dll file in the project folder where the executable is.