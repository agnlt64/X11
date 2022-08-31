# X11
X11 library but easy to install

# Setup
You first have to clone this repo:  
 ```
 git clone https://github.com/ABFStudio/X11
 ```
 Since there are no dependencies, you don't have to build anything from source. Then you can copy all these files into a folder called "X11" and put this
 folder to your project's root. This works as the classic X11 library. However, I recommend installing the classic X11 package.   
 With Homebrew in macOS:  
 ```
 brew install libx11
 ``` 
 Or in Linux (Debian based):  
 ```
 sudo apt install libx11-dev
 ``` 
 
 # Build your project
 On macOS, you have to link the library when compiling. If you have installed X11 with Hombrew, the full path may be `/opt/homebrew/Cellat/libx11/X11VERSION/lib/libX11.6.dylib`. You can check if you are not sure. Then to compile:  
 ```
 g++ main.cpp path-to-x11-lib -o myprog
 ```  
 On Linux, you simply have to link X11:  
 ```
 g++ main.cpp -lX11 -o myprog
 ```
 And that's it! Please note that I will not be maintaining this repo, so feell free to make a PR if something is wrong.
