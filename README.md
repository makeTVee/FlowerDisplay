# FlowerDisplay v0.9
LED flower display based on 8-LED-ring panel

No specific controller needed, any Arduino/Pixelblaze/Pi Pico etc. possible. But there are dedicated pads to directly solder a Pixelblaze Pico to the panel. So the following process descibes the assebly with a Pixelblaze Pico. Other controllers are mentioned at the end.

Before starting the process, you have to remove the stand by slightly bend it ti the side to snap it out of the holes. Then you can pop out the PCB and diffusor. Try to not push directly on the flowers.

1. Add a pinheader to the Pixelblaze Pico
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/ace7e3d2-4ccf-4708-9c0a-27f8771aba0b)

2. Solder the Pico to the FlowerMatrix PCB as shown
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/37f89998-03cf-426d-b277-f18d95af116c)

3. Cut the pins on the front to less than 1mm so they don't protrude above the white diffusor panel.
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/d0e721c5-0a67-4234-834c-0bd2bc9499f6)

4. Make sure the pins are not longer than 1mm 
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/6cd11524-f881-4f95-8b32-33dd1d0beee6)

5. Flower power
   Add a 5V power supply and cut the wires on the front in the same way. There is a cutout in the white diffusor.
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/71438997-9fc9-4f59-b537-f96211bc0225)

7. Snap all back in into the frame and add the stand. Make sure, the display is aligned with the frame as shown for correct mapping.
![image](https://github.com/makeTVee/FlowerDisplay/assets/18531000/b9d752ae-39e3-4f05-833a-50d8bd3a0f0f)

Pixelblaze mapping:
```
[
[17,98],[15,93],[10,91],[5,93],[3,98],[5,103],[10,105],[15,103],
[17,76],[15,71],[10,69],[5,71],[3,76],[5,81],[10,83],[15,81],
[17,54],[15,49],[10,47],[5,49],[3,54],[5,59],[10,61],[15,59],
[17,32],[15,27],[10,25],[5,27],[3,32],[5,37],[10,39],[15,37],
[17,10],[15,5],[10,3],[5,5],[3,10],[5,15],[10,17],[15,15],

[25,10],[27,15],[32,17],[37,15],[39,10],[37,5],[32,3],[27,5],
[25,32],[27,37],[32,39],[37,37],[39,32],[37,27],[32,25],[27,27],
[25,54],[27,59],[32,61],[37,59],[39,54],[37,49],[32,47],[27,49],
[25,76],[27,81],[32,83],[37,81],[39,76],[37,71],[32,69],[27,71],
[25,98],[27,103],[32,105],[37,103],[39,98],[37,93],[32,91],[27,93],

[61,98],[59,93],[54,91],[49,93],[47,98],[49,103],[54,105],[59,103],
[61,76],[59,71],[54,69],[49,71],[47,76],[49,81],[54,83],[59,81],
[61,54],[59,49],[54,47],[49,49],[47,54],[49,59],[54,61],[59,59],
[61,32],[59,27],[54,25],[49,27],[47,32],[49,37],[54,39],[59,37],
[61,10],[59,5],[54,3],[49,5],[47,10],[49,15],[54,17],[59,15],

[69,10],[71,15],[76,17],[81,15],[83,10],[81,5],[76,3],[71,5],
[69,32],[71,37],[76,39],[81,37],[83,32],[81,27],[76,25],[71,27],
[69,54],[71,59],[76,61],[81,59],[83,54],[81,49],[76,47],[71,49],
[69,76],[71,81],[76,83],[81,81],[83,76],[81,71],[76,69],[71,71],
[69,98],[71,103],[76,105],[81,103],[83,98],[81,93],[76,91],[71,93],

[105,98],[103,93],[98,91],[93,93],[91,98],[93,103],[98,105],[103,103],
[105,76],[103,71],[98,69],[93,71],[91,76],[93,81],[98,83],[103,81],
[105,54],[103,49],[98,47],[93,49],[91,54],[93,59],[98,61],[103,59],
[105,32],[103,27],[98,25],[93,27],[91,32],[93,37],[98,39],[103,37],
[105,10],[103,5],[98,3],[93,5],[91,10],[93,15],[98,17],[103,15]
]
```

