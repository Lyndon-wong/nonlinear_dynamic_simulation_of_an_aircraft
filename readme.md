# nonlinear_simulation_of_an_aircraft

# About

This project is a homework project for the course: *Modern Flight Control Systems*, Dr. Bei Lu, Spring, 2021. Based on Simulink, this project established a six-degree-of-freedom nonlinear model of the aircraft and balanced it to obtain a stable flight state. In this state, linearization and dynamic stability analysis of the model were carried out. Finally, the differences between the linearized model and the nonlinear model were compared.

# Overview

![image-20210405213843371](https://gitee.com/lyndon-wong/blogimg/raw/master/image-20210405213843371.png)

# How to use

1. load "sheet.mat".
2. check the model: the trim mode should be connected. Then you can use the trim function in the shell to find the desired stable state. You can use

```[x,u,y] = trim('unlinearized',xi,ui,yi,[],[],[]) ```

and also

```[x,u,y] = trim('unlinearized',xi,ui,yi,[],[],[2,3,4,5,6,7,8,9])```

A recommended state has been set in xi, yi, ui.
3. check the model: the test mode should be connected.
4. run the model and you can see the result in graph.
5. You can change the input as you like in test mode.

# Notice

1. Matlab2020a or up version is required.
2. There is also a linearized for you to compare.

