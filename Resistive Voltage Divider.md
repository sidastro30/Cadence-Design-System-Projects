 # Layout and simulation 
 
 ## Virtuoso Analog Design Environment
 ![image](https://user-images.githubusercontent.com/81389879/180942846-4badda21-4efd-4991-a510-b541f64b54b7.png)
 
 ## Transient Response
 ![image](https://user-images.githubusercontent.com/81389879/180943037-72594b70-b8d8-4d29-836f-5abf0ca59eea.png)
 
 ## Virtuoso Schematic Editor
 ![image](https://user-images.githubusercontent.com/81389879/180943924-50b747f1-5fac-419a-9434-2a09f1d2a2ea.png)
 
 ## Virtuoso Symbol Editor
 ![image](https://user-images.githubusercontent.com/81389879/180944782-2059d525-82f5-43c5-9171-12e62b5447ad.png)
 ![image](https://user-images.githubusercontent.com/81389879/180945192-fca31849-9876-4c81-bd58-23d971781d5b.png)
 
 ## Virtuoso Schematic Editor
 ![image](https://user-images.githubusercontent.com/81389879/180945439-a037a0e2-d280-41dd-9b22-ea5a6f3fcbd0.png)
 ![image](https://user-images.githubusercontent.com/81389879/180945584-868870f2-2b76-4a45-affc-8c10434bbe3f.png)
 
 ## Virtuoso Layout Suite 
Using the n-well layer for the 10k resistor.
The sheet resistance of n-well in the C5 process is roughly 800 ohms.  
The minimum width of n-well is 12 lambda (3.6 microns since lambda here is 300 nm) so let’s make a 10k resistor using a width of 4.5 um and a length 56 um.

![image](https://user-images.githubusercontent.com/81389879/180947951-9cb8f89e-e819-478f-ba03-2c23cc301083.png)

Create a cell (layout view) called R_n_well_10k.
![image](https://user-images.githubusercontent.com/81389879/180946600-2e4fba30-a593-4e0e-89fb-17600064623f.png)

#### connections to the ends of the n-well resistor

![image](https://user-images.githubusercontent.com/81389879/180947556-4f2ccd6b-54f9-45c7-879b-f154bc4bdaf5.png)
![image](https://user-images.githubusercontent.com/81389879/180947701-c2cecf29-5527-42a0-a0f6-2c0f90b32de1.png)

## Layout
![image](https://user-images.githubusercontent.com/81389879/180948431-1d75ec93-3897-4fa6-8054-17b04408297d.png)

### Value verification of single layout resistance
![image](https://user-images.githubusercontent.com/81389879/180948657-3c7d78a8-d204-4ba5-b676-939ae1d6b5e9.png)

### On selecting the metal1 layer in the LSW and add rectangles to connect the resistors together and to connect to the Pins of the resistors. 
![image](https://user-images.githubusercontent.com/81389879/180949203-44faa283-a66f-4d0f-baa3-0403100b1964.png)

##### Pressing e and set the Stop Depth to zero results in showing the outlines of the cells.
![image](https://user-images.githubusercontent.com/81389879/180949510-a3470230-d723-44a7-962b-2718c4065081.png)

#### Adding Pins on the metal1 layer named in, out, and gnd. Set the rectangle size of the Pin to the same size as the metal1
![image](https://user-images.githubusercontent.com/81389879/180949841-d4759499-1a18-4560-be85-33e4bbd47dba.png)











