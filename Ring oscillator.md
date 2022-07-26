# Design, layout, and simulation of a ring oscillator
![image](https://user-images.githubusercontent.com/81389879/181049787-d03862cc-b865-497b-a31e-c294759f4aaf.png)

Instantiate the (first copied) inverter on the output of the existing inverter.
Repeat for the second copied inverter to get the following.
Note that if required a wire between the inverters we could have added the wire on the output of the first inverter and then copy both the inverter and wire.

![image](https://user-images.githubusercontent.com/81389879/181050125-3b309485-be13-42d7-a199-3e45d675b337.png)
![image](https://user-images.githubusercontent.com/81389879/181050292-8e842dce-d5b4-4418-a143-0ff233715482.png)

![image](https://user-images.githubusercontent.com/81389879/181050678-9cdb0488-e319-41f7-b12f-8b8dbf16f7a2.png)

The output is steady at 2.5V!
In a real circuit noise would kick-start the oscillations.
Observation in the simulation by adding an initial condition as follow.

![image](https://user-images.githubusercontent.com/81389879/181051161-8c88e54c-3ddd-43e1-a766-a8d675f52cea.png)

### Making the schematic more simplified.
Delete all of the inverters and the wires except for the first inverter.
Change the inverters name from I0 to I0<1:31> (an array of 31) and display the name (value).

![image](https://user-images.githubusercontent.com/81389879/181051905-425f464e-a645-4835-b2e2-be9296e55a80.png)

#### Layout view for the ring oscillator and place two inverter layouts in the cell next to each other.
![image](https://user-images.githubusercontent.com/81389879/181052278-2fc5dfc3-cbe3-4b22-a948-5128901cf737.png)

#### Set the stop display level back to 10 and delete the right inverter.
![image](https://user-images.githubusercontent.com/81389879/181052582-ba707b2f-839f-49f3-8e42-91c0768409ed.png)

On press c (to copy) and select the entire layout.
Press F3, special options, and set the number of columns to 30

![image](https://user-images.githubusercontent.com/81389879/181052908-7b096c7a-2c57-430b-b1b6-8335850f73af.png)

Next add a rectangle on metal2 connecting these two vias.
Below is the result where the stop display level is set to 0.

![image](https://user-images.githubusercontent.com/81389879/181053136-afdecb82-2764-4548-94b8-0aa1b3a4f235.png)

Add pins for gnd!, vdd! (both have a direction of inputOutput), and osc_out (set the direction to output).
Put vdd! and gnd! pins on the metal1 layer and osc_out on the metal2 layer.

![image](https://user-images.githubusercontent.com/81389879/181053296-dadde13c-5af6-4904-8f35-547fef5d6709.png)

## Symbol Creation
![image](https://user-images.githubusercontent.com/81389879/181053673-b5181571-00b7-4d2d-8e20-2994f264479f.png)
![image](https://user-images.githubusercontent.com/81389879/181053699-0a88a673-baaa-48a5-8c9f-d6115bcd0f5d.png)
![image](https://user-images.githubusercontent.com/81389879/181053881-6a7cf00b-08b3-4d40-bdda-aa371e52828d.png)

#### After Simulation
![image](https://user-images.githubusercontent.com/81389879/181054076-f5040c67-be05-4a03-b24c-dbc8c1a507d3.png)














