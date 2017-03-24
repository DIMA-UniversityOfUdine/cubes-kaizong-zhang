                                                        Introduction
Because I am a Chinese student learn this for the first time, so I'm going to from the simple design of mount, I designed a composed of 
aircraft and the sea scene, make the sea has a certain animation effects,At this point, about i need to choose whether to add a terrain or 
create a short movie,I choose to create a short movie.In the Update function, using the Date.now() Javascript function i can check how
much time is passed since the application started and then activate the correct camera animation.May also have other interesting things to 
add later, the code is contained in index.html file.
                                                         Result
The animation of the sea will be repeated, with light, produce the effect of waves, the plane's propeller movement, looked like the aircraft 
has been in the flight.
                                                         Process
                                                         
20/03/2017
Design and thinking about how to use the cube to produce the effect of the ocean wave,define all kinds of variables, we don't need to write
a <canvas>label,Just need to define a div element in canvas can be loaded, canvas is dynamically generated, the definition of data.now () 
function.Add a scene. Cameras, the renderer and lights,Light setting can create a feeling of sunlight.
21/03/2017
Add cockpit,engine and TailPlane.A cube, for example, can be modified by moving its vertices. In our case we want to make it look more like a cockpit.can access a specific vertex of a shape through the vertices array, and then move its x, y and z property.
22/03/2017
Add SideWing,Propeller,Blade.
23/03/2017
Using the cube to create the prototype, the use of MeshPhongMaterial to each the color Settings,incude ambient,(Set the material environment).emissive(Set up the launch of the color material),specular(Specify the material of light and the color of the highlight part).
24/03/2017
To complete the code of this part of the sea, to produce the effect of wave, use computeMorphNormals method and the Vertex Normal method, Using trigonometric functions and timer to define the number of times and cycles.
