# Ros 2 Pycharm Intellisense Fix
Solution for libraries import unresolved reference error in Pycharm with Ros 2 with/without Docker:

## Table of contents
* [Problem](#problem)
* [Solution](#solution)
  * [Add Python interpreter from Docker](#add-python-interpreter-from-docker)
  * [Add Ros 2 libraries](#add-ros-2-libraries)


## Problem

Pycharm Intelisense doesn't see ROS 2 Python libraries

![Screenshot](screens/others/problem.png)


## Solution


### Add Python interpreter from Docker

Click **File** in left top corner near Pycharm logo

![Screenshot](screens/docker/step1.png)

Click **Settings**

![Screenshot](screens/docker/step2.png)

Choose your project

![Screenshot](screens/docker/step3.png)

Click **Python interpreter**

![Screenshot](screens/docker/step4.png)

Click on actual Python interpreter

![Screenshot](screens/docker/step5.png)

Click on **Show All...**

![Screenshot](screens/docker/step6.png)

Click on **+** in new window

![Screenshot](screens/docker/step7.png)

Click **On Docker**

![Screenshot](screens/docker/step8.png)

In **Image** options choose **Pull or use existing**

![Screenshot](screens/docker/step9.png)

In **Image Tag** write your image name

![Screenshot](screens/docker/step10.png)

Click <kbd> <br> Next <br> </kbd>

![Screenshot](screens/docker/step11.png)

Wait for image pulling and click <kbd> <br> Next <br> </kbd>

![Screenshot](screens/docker/step12.png)

Click <kbd> <br> Create <br> </kbd>

![Screenshot](screens/docker/step13.png)

Click <kbd> <br> OK <br> </kbd>

![Screenshot](screens/docker/step14.png)


### Add Ros 2 libraries

Click on **Show All...** in Settings

![Screenshot](screens/libraries/step15.png)

Click on strange folder branch icon near hopper in new window

![Screenshot](screens/libraries/step16.png)

Click **+** in new window for every path (more in next step)

![Screenshot](screens/libraries/step17.png)

Enter 2 paths in the same way separetly with this template:

```
/opt/ros/<ros-distro>/lib/<python-version>/site-packages/
```

```
/opt/ros/<ros-distro>/local/lib/<python-version>/dist-packages/
```

![Screenshot](screens/libraries/step18.png)

On next screenshot there are examples of paths.

After adding two path separetly click <kbd> <br> OK <br> </kbd>

![Screenshot](screens/libraries/step19.png)

In Python Interpreters click <kbd> <br> Apply <br> </kbd>

![Screenshot](screens/libraries/step20.png)

Next click <kbd> <br> OK <br> </kbd>

![Screenshot](screens/libraries/step21.png)

In Settings click <kbd> <br> Apply <br> </kbd>

![Screenshot](screens/libraries/step22.png)

and then click <kbd> <br> OK <br> </kbd>

![Screenshot](screens/libraries/step23.png)

After that you need wait for index (on bottom of the Pycharm)

![Screenshot](screens/others/indexing.png)
