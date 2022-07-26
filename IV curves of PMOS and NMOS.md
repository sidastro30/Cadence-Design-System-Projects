# Layout and Simulate operation of NMOS and PMOS transistors using the C5 process
# NMOS
## Virtuoso Schematic Editor

![image](https://user-images.githubusercontent.com/81389879/180953635-480d3ffd-bd73-4ea4-bef2-f773704be741.png)

![image](https://user-images.githubusercontent.com/81389879/180954313-757aae71-a770-4d56-b953-abcebf5632a2.png)


Instantiate the NMOS_IV_Cell View just created and the DC voltage sources

![image](https://user-images.githubusercontent.com/81389879/180954707-e8cd62bf-ee52-40f8-b6bd-555995ae9e44.png)


Parametric Analysis window, to see the MOSFET IV curves

![image](https://user-images.githubusercontent.com/81389879/180959759-1a6dbcbb-6df9-4018-9fb2-b48302222286.png)

![image](https://user-images.githubusercontent.com/81389879/180960082-07bcd093-4e87-4056-82da-c6f0ac218c0c.png)

## Virtuoso Layout Suite 
### Instantiate an nmos device that is 6 um wide and 600 nm long

Next instantiate a ptap cell (metal1 connection to p+) in the p-substrate

![image](https://user-images.githubusercontent.com/81389879/180960662-a23a7e7f-1455-4cc6-851e-71ecf01853a3.png)


Next add rectangles on the metal1 layer to connect the source to the p-substrate and to the drain.
Also add a metal1-connection-to-poly cell (m1_poly) and a poly rectangle to connect the gate to m1_poly.

![image](https://user-images.githubusercontent.com/81389879/180960890-dc9cc985-7d7e-418b-8495-89ed74e55780.png)


Pressing e and then setting the display level stop to 0 we can see the rectangles and cells

![image](https://user-images.githubusercontent.com/81389879/180961059-b24ded96-e4cc-480e-b4fc-41f45a277f18.png)


Add D, G, and S Pins on metal1

![image](https://user-images.githubusercontent.com/81389879/180961462-e1924715-ac7c-412e-be56-eedd8fec0ae1.png)


## Extracted cell view

![image](https://user-images.githubusercontent.com/81389879/180961676-a2f0cc1e-2a25-40f2-a051-ec467ec9be45.png)


```
Notice that the symbol displayed here has 4 terminals, not the 3-terminal transistor we used in the schematic (where it’s assumed the p-substrate is tied to gnd!)
Next run an LVS

The error is related to the bulk (p-substrate) connection for the NMOS. Again, as mentioned above when the 3 terminal MOSFET symbol is used it’s assumed
that the bulk is tied to gnd! for an NMOS device and vdd! for a PMOS device.
Let’s modify the layout as seen below.
Delete the metal1 rectangle and pin connecting the S to the bulk (ptap) as seen below
```
![image](https://user-images.githubusercontent.com/81389879/180962790-01f15c2c-3ff0-4423-828d-87e541742838.png)

On adding  metal rectangles on metal1 over the S and B metal

![image](https://user-images.githubusercontent.com/81389879/180962991-3649234e-61f4-47a2-9805-71c775c7ac26.png)


Next add Pins, again make the Pin the same size as the metal1 rectangles

![image](https://user-images.githubusercontent.com/81389879/180963204-2a8818c5-66b8-4205-8d01-196f42cb8c72.png)

Extracted view using the Library Manager.
Notice that it’s basically the same view except that now the bulk of the NMOS devices is connected to gnd!

![image](https://user-images.githubusercontent.com/81389879/180963465-846a1559-1b83-42f2-bdfe-9ab964258f05.png)



# PMOS
Repeat these steps for the PMOS device but in a much more concise manner.
Create a schematic Cell View called PMOS_IV with 4 pins as seen below. Note the W and L of the PMOS device

## Virtuoso Schematic Editor

![image](https://user-images.githubusercontent.com/81389879/180964332-8a7d85db-690b-477e-b1d3-1937f7c0e63d.png)

![image](https://user-images.githubusercontent.com/81389879/180964656-d60991e2-e153-4967-93f5-25343b782eae.png)


## Virtuoso Layout Suite 
### Layout (pmos cell and ntap)

![image](https://user-images.githubusercontent.com/81389879/180965091-682256f6-dc5e-48cb-8ef2-0b6d00b797e8.png)


## Extracted cell view

![image](https://user-images.githubusercontent.com/81389879/180965212-93e6fa99-7ad7-478a-9c33-172f429d5048.png)

Next create a cell called sim_PMOS_IV and draft the following schematic.
Note the value of /V1 is VSG (not VGS as we used in the NMOS sim).

![image](https://user-images.githubusercontent.com/81389879/180965682-033552f6-7914-4666-a87b-276cfce69809.png)

Simulation of the schematic

![image](https://user-images.githubusercontent.com/81389879/180965892-3fe92e38-afb5-46dc-ac96-47981eb2652a.png)

![image](https://user-images.githubusercontent.com/81389879/180966440-0a34bea1-0dd1-40c5-b20a-f5c1d49fe840.png)








