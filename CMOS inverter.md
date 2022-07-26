Schematic, Symbol, Layout and simulate the DC behavior of the of a CMOS inverter.

## Virtuoso Schematic Editor

![image](https://user-images.githubusercontent.com/81389879/181022850-285a2e8a-60c0-4182-9eb1-f55806baf0e9.png)

Adding the following cells (nmos, pmos, ntap, ptap, and m1_poly) to layout view as seen below (you can copy as before but here we will instantiate cells).
Ensure the nmos is 6u/0.6u and pmos is 12u/0.6u and the ntap and ptap use two columns.

![image](https://user-images.githubusercontent.com/81389879/181024094-9944bc72-6bd0-4fd4-9263-996b0f2fd8fc.png)

Aligning the cells

![image](https://user-images.githubusercontent.com/81389879/181024248-8911fc7d-a787-4a19-8018-07ca8a3d5ae3.png)


Adding rectangles on poly and metal1

![image](https://user-images.githubusercontent.com/81389879/181025261-92c69023-3a36-429e-9afc-d1742101ccc9.png)

![image](https://user-images.githubusercontent.com/81389879/181025548-0fcc2334-f709-428b-adc9-f14c212ec47f.png)

![image](https://user-images.githubusercontent.com/81389879/181025373-53c1aee2-5208-4bd5-8291-2e6be365bdec.png)


Adding pins on metal1 for gnd!, vdd! (both have a direction of inputOutput), A (input), and Ai (output).

![image](https://user-images.githubusercontent.com/81389879/181025849-5e103605-16f4-4557-81dc-b70097d86b12.png)
![image](https://user-images.githubusercontent.com/81389879/181025967-bb4c1194-d012-432f-933e-f142ee278994.png)

## Extracted

![image](https://user-images.githubusercontent.com/81389879/181026341-c3a913f9-8317-4f7e-aa71-b9ce8c52a4b5.png)
![image](https://user-images.githubusercontent.com/81389879/181026597-190d4544-8f42-433c-835a-c46572874f0b.png)


## Simulation

![image](https://user-images.githubusercontent.com/81389879/181027049-a3dd52e1-0e1f-4761-91c7-23fcd3d98ba3.png)


Expected the inverter voltage transfer curves

![image](https://user-images.githubusercontent.com/81389879/181027699-813e536a-8575-464e-afef-bb11e89e203b.png)







