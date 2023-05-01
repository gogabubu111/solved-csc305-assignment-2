Download Link: https://assignmentchef.com/product/solved-csc305-assignment-2
<br>
In assignment 2, we will create a small procedural terrain based on Perlin noise, texture the terrain based on height, and place some objects on the terrain following the local normal vector of the terrain.




(Note: Demo picture on the right is created with a 4×4

random gradient grid and no fractals.)




Assignment 2 and 3 are divided into two parts. Correctly completing all features the ​<u>Basic</u> <u>Requirements</u>​ part will award you a grade ​<u>up to 70%</u><u>​</u> of the assignment. To get <u>​100%</u><u>​</u>, you must selectively implement a few features in the <u>​Advanced Requirements</u><u>​</u> part, whose solutions are not completely covered in lectures and requires original research. The Advanced Requirements are open-ended, and you are welcomed to propose and work on your own preferred features. You should come to discuss your own idea with the TA or the instructor <u>​first</u><u>​</u>; and point values will be assigned to your proposed feature after we discuss it.




When you submit your assignment 2 and 3, you need to include a list of feature points that you claim you have completed, and your TA will ask you questions about all feature points you listed during the grading lab session. Downloading an existing Unity package/asset for a feature is not considered as completing that feature by yourself.




<h1>Assignment 2 – Basic Requirements (70%)</h1>

<ol>

 <li>Generate a square Perlin noise patch with sampling resolution 250×250. Tune the frequency and amplitude of the noise to yield appealing results. (Hint: if you aren’t sure what was the result of your Perlin noise generator, you can visualize this 250×250 2D float array as an image using the code from Assignment 1) (20%)</li>

 <li>Generate a plane mesh that’s divided into a 250×250 grid, with each grid cell’s rectangle conventionally divided into 2 triangles. (10%)</li>

 <li>Using the Perlin noise patch generated in step 1 as a ​<u>height map</u>​, elevate vertices generated in (2) to form a procedural terrain. (10%)</li>

 <li>Write a vertex/fragment shader pair of the terrain, which can texture the procedure terrain with at least 4 different textures according to height. (Hint: You must compute the height in the object space of the terrain model, which means if you move your terrain mesh up and down in the Scene Editor, the texture distribution does not change). (10%)</li>

 <li>Implement the Phong-Blinn reflection model in the fragment shader, treating the texture colour as surface albedo (Hint: you need camera position in the fragment shader for specular reflection). (10%)</li>

 <li>Place a few 3D models onto the procedural terrain, elevate them as the terrain goes up, and rotate them so they seem to be upright on their local surface. (Hint: you need to calculate the local ​<u>normal</u><u>​</u> of the procedure terrain). (10%)</li>

</ol>




<h1>Assignment 2 – Advanced Requirements (up to 30%)</h1>

<ul>

 <li>Add fractal Perlin noise to the heightfield and create height variation details on different scales. (5%)</li>

 <li>Make a moveable camera so you can fly through the scene and examine your terrain from any point of view. (5%)</li>

 <li>Scatter more models on to your mini-terrain, for example, other houses and little towers. When place then randomly, write code to ensure that they don’t overlap each other. (5%)</li>

 <li>Extend the procedural terrain to infinity (or to a very large area such that it looks like infinite) while keeping a reasonable rendering performance. (10%)</li>

 <li>Add reflections to the water that not only reflects the skybox but also the mountains/placed 3D models above the water. (10%)</li>

 <li>Add ripple effect to the water. (5%)</li>

 <li>Desaturate everything in the scene according to a fragment’s distance to the camera, such that far away terrain &amp; objects appear grey-ish and things closer to the camera have more vibrant colour. (Hint: you need a method to adjust a pixel’s saturation only, without changing its hue or luminance.) (10%)</li>

 <li>Add moving sun and clouds in the skybox, create a day/night cycle. (10%)</li>

 <li>Create atmospheric rendering effects for the environment – adjust the sunlight colour, cloud colour, reflection and shadows according to the simulated time of the day and the sun’s height from the horizon. (10%)</li>

 <li>Add interactive terrain editing features: when a user clicks on part of the terrain, s/he can use the mouse to drag the terrain up and down. Surface features such as water definition, texturing and small models must be updated in real time according to the editing. (10%)</li>

 <li><u>Feel free to propose your own ideas and improvements for Advanced Requirements.</u> Your instructor/TA will assign a point value after discussing the idea with you.</li>

</ul>


