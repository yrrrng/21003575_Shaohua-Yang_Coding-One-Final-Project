# 21003575_Shaohua-Yang_Coding-One-Final-Project

Video Link：https://www.youtube.com/watch?v=3Su8uaxFXRI

Mimic Link：https://mimicproject.com/code/aae980bf-1843-11c8-693c-902b548f4f01

Time passes in different directions, and these pixels often face another transformation of form as time goes by. Although we can watch its transformation from different angles, it is not able to change its dissipating trajectory. The aim of this project is that everything is diverse, just as when we use the mouse to place different points in the coordinates, each point takes on a different color and shape.

In this project I used a combination of audio oscillators and shaders, I used the snowflake screen as the inspiration, the mouse as the input interaction event, and the shaders as the different colors and shapes over time. When building the shader, I referenced mouse, time, and resolution as inputs and used random and graphical noise to randomize the graph, then I converted the floating-point values to colors and did a linear superposition of the 4 gradient values to form the noise graph, and I referenced time and mouse as nested within the color when the shader color as output. in. The mouse shows different color changes at different points and combined with the time and mouse inputs create a sense of time passing. I then used the audio oscillators maxiAudio and myOsc to import the sound from the snowflake screen and combined it with the drum changes to finally bring in the sound. I then generated random materials based on the Three.js method by defining the mesh method combined with the shader, built the 3d scene by defining the scene, camera, and other elements, and then generated random path indices with vertex shaders, slice shaders, and pixel shaders. This is followed by a render method that listens to any changes in the scene in real time, thus achieving the ability to render the scene in real-time. Also, in terms of compatibility, the resizeWindow method allows for timely adjustment of view, camera, and scene parameters as the listener window changes.

The shortcoming of this project is that the music noise needs to be combined with fluctuations and rhythms so that the fluctuations between the snow screen and the sound can be shown more graphically, and in conjunction with the mouse to achieve different axis changes, what sound will be produced when there are more manic points and what sound will be produced when there are fewer, which is something I need to think about in the future.
