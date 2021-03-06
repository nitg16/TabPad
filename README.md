# TabPad 
TabPad is an onscreen gamepad for Linux touchscreen devices (mainly tablets).

# Screenshots
![alt text](https://raw.githubusercontent.com/nitg16/TabPad/master/TabPad.jpg)
![alt text](https://raw.githubusercontent.com/nitg16/TabPad/master/TabPad1.png)

# Installation 
    sudo apt install python3-pyqt5 xdotool xinput python3-pip
    sudo pip3 install PyUserInput 

# Running TabPad 
Run the command below to launch TabPad.

    python3 TabPad.py 

# Configuring TabPad  
Edit `TabPadConfig.py` file.

# FAQ
**<u>Why TabPad is Not Transparent?</u>**

TabPad transparency depends on your compositing manager. If the compositing manager do not support transparency, you may see an opaque or a translucent background. TapPad works absolutely fine with Compiz, Mutter and Kwin.

**<u>Why TapPad layout is weird with overlapping buttons?</u>**

If you have changed orientation, restart the app. Otherwise read below.  

TabPad comes with a default layout. However different tablets with different screen sizes and resolution exist and it is difficult to define one standard layout. Further, the layout also depends on overlay geometry you define in `TabPadConfig.py` file.

The best possible way to solve it is to change button position and size in `TabPadConfig.py` file as per your requirements.   

# Current Limitations 
  * ~~Diagonal movement keys are yet to be implemented.~~
  * Works only in games running in windowed mode (no fullscreen support yet).
  * TabPad may not work properly in portrait mode. Support for portrait mode will be improved once all features are implemented for landscape mode.
