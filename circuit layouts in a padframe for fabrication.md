# Circuit layouts in a padframe for fabrication
```
If  12 pad cells on a side (10 plus two corners) then each cell must be 1.5mm/12 or 125 um.
In order to ensure this pad falls on the 0.15 um grid let’s reduce the pad cell size to 120 um.
This also ensures that the final chip size is smaller than the 1.5 mm square size we are allowed.
```
## Pad Layout
![image](https://user-images.githubusercontent.com/81389879/181056132-eaf00ca7-ca0a-453c-bf65-c51c1250a735.png)


Add a wide wire with a label pin<1:40>

![image](https://user-images.githubusercontent.com/81389879/181056869-d079546b-1e92-4e2d-bd3a-0d5c27def175.png)
![image](https://user-images.githubusercontent.com/81389879/181057047-431781d8-5e0f-4d28-b97b-1382c42b8ddf.png)


Create a schematic view of a cell called “chip” and add the cells previously created.
Wire the cells up as seen (an arbitrary connection).
Note how we’ve used pin<20> for ground and pin<40> for power.

![image](https://user-images.githubusercontent.com/81389879/181057165-967a0268-71a8-4fa8-948f-9d69536bed8c.png)

Connect the cells up to the padframe in the layout.
Create of layout view of the “chip” cell.
Place the R_div, NMOS_IV, PMOS_IV, inverter, nand2, and ring oscillator cells near the pads that they will connect to, below.
Adjusting the cells positions as needed and focus on wiring the circuits to the padframe.

![image](https://user-images.githubusercontent.com/81389879/181058131-6ff8201b-b578-4479-a0b3-a5dc4517dd63.png)

Adding rectangles on the metal layers to move towards connecting the cells up to the padframe.
Zoomed view in around the ring oscillator and resistive divider.

![image](https://user-images.githubusercontent.com/81389879/181058530-80327e54-8b45-4034-bd9d-56268885eb8a.png)
![image](https://user-images.githubusercontent.com/81389879/181058669-11cd72ef-9d08-4127-a52c-f0e1f309ae55.png)

### Full connected view
![image](https://user-images.githubusercontent.com/81389879/181058875-8d256c0e-42c5-4fab-a34b-1cb66c516586.png)
![image](https://user-images.githubusercontent.com/81389879/181059437-f56dfaf6-7418-462c-9c00-714134125e1f.png)
![image](https://user-images.githubusercontent.com/81389879/181059521-0e403877-068d-4e7f-bbe0-434ae9d40a9a.png)

### Extracted the layout view
![image](https://user-images.githubusercontent.com/81389879/181059112-4f54b69c-7552-4f7e-982d-114766168458.png)








