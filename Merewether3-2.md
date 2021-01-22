#### Water depth or water surface elevation output files (`-xxxx.wd`, `-xxxx.elev`)

In these files, a 2D grid of water depths (`.wd`) and water free-surface elevations (`.elev`) values (in meter) will be written. The data will be written in these files with the same ASCII raster format of the DEM input file at each save interval, `saveint`, as specified in the `.par` file. 

Based on this naming convention, `xxxx` is the `saveint` number. For instance in the example of Merewether test case, since `saveint` is 10 seconds, `merewether-0002.wd` will contain the water depth output at t = 20 seconds. It should be reminded that generation of `.elev` files will be suppressed by including the keyword `.elevoff` in the `.par` file. In case of the DG2 solver two extra files named `-xxxx.wd1x`, `-xxxx.wd1y` or `-xxxx.elev1x`, `-xxxx.elev1y` will be generated that contain the X and Y direction slope coeficient values of water depth and free-surface elevation, respectively.


[back](/Merewether3.md)