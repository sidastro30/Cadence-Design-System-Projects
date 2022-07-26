## Virtuoso Schematic Editor

![image](https://user-images.githubusercontent.com/81389879/181044288-cc594a14-9394-47f0-802e-6359c12584eb.png)


## Virtuoso Symbol Editor

![image](https://user-images.githubusercontent.com/81389879/181044670-8b2714ff-f413-4516-8535-9332d8aa13c8.png)


## Simulation

![image](https://user-images.githubusercontent.com/81389879/181045101-1a307efb-6373-4930-a383-382f5d5819a0.png)
![image](https://user-images.githubusercontent.com/81389879/181045276-24442878-5d8c-4545-8f8f-fb0ff34b9fdb.png)


## Virtuoso Layout Suite
![image](https://user-images.githubusercontent.com/81389879/181045626-70a61146-84b1-4848-9b9b-47f1cd3df2b6.png)

Delete the metal1 and Ai pin connecting the drains of the MOSFETs.
Delete the metal1 connecting the source to the ptap then delete the gnd! pin.
Move the ptap to the left side of the layout.

![image](https://user-images.githubusercontent.com/81389879/181046179-b6b8500d-9dce-47f1-82c9-5b0babbba12c.png)


delete the metal1 from the ntap to the source of the PMOS and delete the vdd! pin

![image](https://user-images.githubusercontent.com/81389879/181047129-80ea9a76-175a-4b67-9824-2dff0ab6bb5b.png)

Move the right pmos until it overlaps the left pmos as seen below.
Change the ntap cell so that it has 5 columns of contacts.

![image](https://user-images.githubusercontent.com/81389879/181047489-8b7de339-c21a-4b42-9b99-7e7d0e3fbc0e.png)


Next change the ptap cell so that it has 5 columns of contacts.
Move the ptap cell so that it is under the nmos cell.

![image](https://user-images.githubusercontent.com/81389879/181047799-82b71633-f0b7-48ae-ab6c-bbe1ce068ea5.png)

Now copy the second nmos and overlap it with the first, like we did above for the PMOS.
Also move the m1_poly and A pin over adjacent to the vertical poly and add a poly rectangle, m1_poly, and B pin (input) for the added PMOS.
Ensure that pin names are showing, the pins are added on metal1. Let’s go ahead and add pins (inputOutput) for vdd! and gnd! while we are at it.

![image](https://user-images.githubusercontent.com/81389879/181048224-490b008b-bea4-4b28-ae56-26e20f1df3ce.png)
```
Removing the metal in between the two MOSFETs.
Select both MOSFETs then flatten them (makes it so the nmos cells are no longer cells but rather rectangles in the layout).
De-select Preserve Pins Geometries.
This ensures that the geometric information of flattened pins is not preserved.

Delete the metal1 and contacts between the two nmos.
Add metal1 to gnd!, vdd! (two places), and connect the drains of the two pmos to the drain of the nmos.
Finally, add a pin, AnandB (output direction) as seen below for the final layout.
```
![image](https://user-images.githubusercontent.com/81389879/181048877-7df04a72-94a8-4db9-9614-8d1d861b37a5.png)




