# GDOP_Calculations

Python script that calculates GDOP at various elevations (we define elevation as perpendicular distance to the Earth-Moon plane, the plane that contains the Earth, Moon, and Lagrange points). Some sample outputs are below:

![0km](https://github.com/abaranov25/GDOP_Calculations/assets/99375046/88e7a4e1-1c14-4d96-9245-dd0892284122)
![100000km](https://github.com/abaranov25/GDOP_Calculations/assets/99375046/66f5d28d-74ef-4919-b935-d10b6699b72a)
![1000000km](https://github.com/abaranov25/GDOP_Calculations/assets/99375046/009c733a-5e89-45c5-addf-c525ceb4d868)

The architecture I used was 24 Earth satellites, 12 Moon orbit satellites, 2 satellites at L2 orbit, and 4 satellites at L4 and L5 orbits. The GDOP can get quite low according to assumptions made, nearing Earth GPS GDOP at certain elevations. One interesting observation is that 0km elevation has high GDOP compared to 100km elevation, which is due to z-axis contributions to GDOP. 

I included the Python script used to generate these plots, so that one can play around with the numbers for additional simulations. One future addition I can make at request is a GIF of how GDOP changes as elevation changes (this would be a 3D heatmap with three slices shown above).
