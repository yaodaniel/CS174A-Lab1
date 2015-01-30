# CS174A-Lab1
These are the folders for assignment 1 of UCLA CS 174A, taught by professor Demetri Terzoupolos.

Our template:

mat.h
vec.h 
	Vector and matrix types and functions.
ArcBall.h
	Mouse control. 
Timer.h
FrameSaver.h
	Recording into frames, which may be used in the second project for video generation.
Shape.h
	Our definitions for the vertices of some primitive shapes.
InitShaders.h
	Reads the shader files and sends the commands to compile them.
	

Your code:

vshader.glsl
fshader.glsl
	Shaders, which determine the appearance of your models.  Defaults are provided.
anim.cpp
	The majority (maybe all) of your coding should happen in here.  A large code skeleton is set up for you.
emcmdprompt.bat
	After you have installed Emscripten from the internet, run this to launch it in your folder.  To produce a WebGL page out of your code enter the following command:
	
		emcc anim.cpp -o hello.html -std=c++11 --embed-file vshader.glsl --embed-file fshader.glsl
		
	Or to have it spend some extra time generating a smaller web page file that almost reaches C++ speeds:
	
		emcc anim.cpp -o hello.html -std=c++11 --embed-file vshader.glsl --embed-file fshader.glsl -Oz -O3 --memory-init-file 0


The first step is to successfully run this template code. Then, study the display() function inside anim.cpp and try to play with it by adding commands.

