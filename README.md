# blankcanvas




Here lie the remains of my GLFW/Vulkan setup for Dear ImGui integration. It was initially intended for my Gymman (Gym-Manager repo on my profile) project. But soon after I started to try and actually implement my database functionality, I realized (far too late because I'm stubborn) that ImGui was never meant to be used for consumer-facing applications.




How silly of me...




Now instead of just scrapping EVERYTHING in this implementation, which was basically me going through a tutorial on how to implement a GLFW/Vulkan renderer, I decided to put that implementation here. Whether it be in case I ever want to use it for something it was actually meant for down the line, or in the case that I would rather it still exist because, IDK, it feels wasteful to delete or something lol.




The project includes copied code from the Dear ImGui repository (by ocornut on GitHub) in `imgui`, a set of rendering boilerplates in `src/render`, an initialization test file `src/test_glfw.cpp`, and `src/main.cpp`.




You will need the following dependencies for Debian: `libvulkan1`, `mesa-vulkan-drivers`, `vulkan-tools`, and `libglfw3-dev`. Soooooooo... I guess here's how to do that lol.




```bash

$ sudo apt update && sudo apt install libvulkan1 mesa-vulkan-drivers vulkan-tools libglfw3-dev

```




And it's just a simple makefile to run it soooooooooooooo.....




```

$ make run

```




Anyone is welcome to use this for whatever; most of it isn't that original, honestly. And a lot of it can be done just by taking some time to read the documentation in the Dear ImGui repo. Have fun :)


