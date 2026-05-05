# USB-HUB
Welcome to a guide to make your own USB 2.0 HUB for less price and get the experience of making a DIY Hardware project.   
This product has a USB-A port to connect to the computer and 4 extra ports, 3 USB-A and 1 USB-C port.  
This guide and the files are open source and completely free to distribute, use, or modify but you are not allowed to sell these files.  
This USB HUB has a transfer rate of 480 Mbs (Megabits per second) or around 60 MBs (MegaBytes per second).  
This is alright for Keyboard, Mouse, Printer, USB Drives, Game Controllers, etc.    
This is not meant for use with High-Speed Devices, or Devices that require a lot of power like RGB-Heavy Devices or High-Power WIFI Adapters.  
Please confirm that everything checks out and I am not liable for any problems with this project. I have made this to the best of my ability and there may be mistakes. Please make an issue in the tabs above for any problems you find.
This guide will only show you how to order online and not solder or print yourself since even I do not know how to do these.


## Files
1. PCB-PCBA.zip is a gerber file which is going to be used to tell the Manufacturing service how the PCB should be made.  
2. Enclosure.obj is an object file which is a 3D Model and it is going to be used to 3D Print the Enclosure.  
3. Source-Project.epro is the PCB source file for any further modifications that you would want to do.  
4. Model.blend is the Blender source file for any further modifications that you would want to do.  
    
    
## Steps
This part of the guide will define an overview of the steps required to end up with a complete USB HUB.
1. Start by downloading the [latest release](https://github.com/Osaidii/USB-HUB/releases) of the files in this repository.
2. You will get the files Enclosure.obj, PCB-PCBA.zip, Source-files.epro, and Model.blend after you extract the files from the zip file. The only ones you need if you are not doing any modifications are the first two.
3. This is the point where if you want to modify the project for yourself, you can do so by skipping ahead to [Modify](https://github.com/Osaidii/USB-HUB#modify) and coming back later and continuing here.
5. Now we can start by placing our order of the PCB (Printed Circuit Board) and the 3D Printed Enclosure.
6. First of all you need to head to [JLCPCB](https://jlcpcb.com/) (which i am using) and create an account. You can also use any other PCB manufacturing service you want to use.
7. Then you need to press Order now and select Standard PCB/PCBA at the top.
8. After this, you will need to upload the Gerber files which is the Order.zip file we downloaded earlier.
9. The only settings we might need to change now are PCB Color and Surface Finish.
10. PCB Color is the color of the chip, in my opinion Green, Black, and Blue look good but you can choose whichever color you want (this only makes a visual difference).
11. For this PCB, you just need to confirm that the settings are set to 2 Layers and 1.6 mm PCB Thickness if not already selected.
12. For Surface Finish, you can select HASL with lead or Lead Free HASL (which I am going to be choosing since it is a little safer).
13. Then you need to scroll all the way down and turn on PCB Assembly and select 5 as PCB Assembly Quantity, now you can also select any coupons from the bottom as there are many coupons that give discounts (you can only select one coupon for one transaction). 
14. Now you would be able to see a table of items in front of you with weird names, you just need to make sure that all of the items are ticked on and turn them on if they are not.
15. Then you can go ahead and keep pressing next and finally press save to cart but do not order now.
16. Now we can go ahead and add our 3D Printed Enclosure in the same order since shipping is quite a lot on JLCPCB.
17. We can press Order now again from the top and Select 3D Printing at the top.
18. Then you can upload the Enclosure.obj file in the first option.
19. You can Research or ask ChatGPT about the 3D Technology and Material but I am going to use SLA (Resin) and 9600 Resin which are the default options and the cheapest ones.
20. Now you can select the Surface finish if you want it, I am going to select General Sanding.
21. For the quantity, The PCBs that we ordered are 5, which is the minimum option for buying from JLCPCB, you can go ahead and select as many Enclosures/Cases you want. I am selecting 2 for Money's Sake.
22. Now you can click save to cart and also go ahead and buy both of the things.
23. The only thing left is screws, we need 3 screws for each case, and we need 2mm x 15mm screws.
24. I am going to buy some of these, but you might be able to find better prices in your region. ############
25. Once you receive all your items, we can go ahead and complete the Whole Thing.
26. First we can take out Side with walls and we can put our PCB upside down so that the Ports line up with the holes for them.
27. Then we can position the PCB so that the PCB holes and the screw standoffs line up (The standoffs are a little smaller purposefully).
28. Now you can place the lid on top of the whole thing and put the screws inside the Holes.
29. Now you can go ahead and screw the screws so that the whole thing locks.
30. The screws might be a little hard to screw since they are self-tapping screws and they might stick out just a little bit.
31. Congratulations, You just completed the USB Hub.
32. Thanks for following this Guide and I hope you are satisfied with the final product.
    
    
## Modification
This part of the guide is going to be divided into two parts.  
1. The PCB  
2. The Enclosure  
  
First of all we are going to start with how you can modify the PCB.  
1. First of all, these PCB files are meant for EasyEdaPro and if you are using other software, please check if these files work with your software.
2. Now, you can head to [EasyEdaPro](https://easyeda.com/) and make an account or login.
3. Then you can click Design Online and then Pro edition since it is a lot easier.
4. Now you can click File -> Import -> EasyEDA(Standard).
5. Now you can select Source-Project.epro which will give you the option to modify and change the Schematics and the PCB.
6. Some things you can add are lights for when a usb is plugged in, Add more Ports, or upgrade the ports from USB 2.0 to 3.0.
7. After you are done modifying, You can press Check DRC in the bottom tab.
8. If there are any things that pop up in the DRC zone, that means there is an error. You can search online, use AI to fix these, or use your brain to fix these.
9. Now we need to export the files in Gerber Format so that we can order the PCB.
10. For exporting, press File -> Export -> PCB Fabrication File (Gerber) -> Export Gerber -> No, continue exporting.
11. Now you have your Gerber files which are the same as PCB-PCBA.zip but include your changes (you can use these files instead of PCB-PCBA.zip, i mean).

Now we are going to do the Enclosure
1. Warning, I used Blender to design this enclosure which is not the standard, it might not be even meant for this use.
2. First you can go to Blender, press
3. If you have modified the size of the PCB, please continue reading, if not please skip to Step 9.
4. Now, you will need to import the PCB into this blender project so that you can fix the size according to the PCB.
5. For this, in EasyEda pro, you can go ahead and press File -> Export -> 3D File.
6. Now you can press OBJ and then export.
7. Back in blender, you can press File -> Import -> Wavefront(.obj) and select this file.
8. Now you have the PCB inside blender so you can make the measurements.
9. After you are done modifying the Enclosure, you can position both Base, Lid and any other parts that you have, Flat side down at the same height.
10. Please just check that these things are alright (Manifolds, Geometry, Normals, and Scale).
11. To check if everything is Manifold / Watertight, select all the Enclosure Meshes (not the PCB) and go to edit mode.
12. Once There, Go to Select underneath the Ribbon with File and Edit, then press Select All by Trait, and then Non-Manifold.
13. If Anything is highlighted, please fix it here.
14. To check that there is no loose geometry, select all the Enclosure Meshes (not the PCB) again and go to edit mode.
15. Once there, Go to Select underneath the Ribbon with File and Edit, then press Select All by Trait, and then Loose Geometry.
16. If anything is highlighted, please fix it here.
17. To check for Internal Faces, Press Z and Wireframe in Object mode.
18. Check if there are any faces inside the Meshes.
19. Then Press A -> M -> By Distance.
20. Now, in Object mode, you need to go to the circles at the top right of the viewport, there are two overlapping circles near it, press the circles and then enable Face Orientation.
21. Everythings should be Blue, if anything is red, You need to flip it,
22. To Flip any Faces, Go to Edit Mode, Select the Face and press Shift + N, and then Flip.
23. Do this for all red Faces.
24. If you have used any Booleans, Mirrors, or even Unions, Apply the Booleans, and try to fix the self-intersections, if not possible, rebuild the area or search for different ways to make that part.
25. Finally, just make sure your Project is set to millimeters in Inspector -> Scene -> Units -> Length -> Millimeters.
26. Now you are done checking your model for problems.
27. Then you can delete any things that you do not need, and then press File -> Export -> Wavefront(.obj) and save the file
28. Now this file is basically Eclosure.obj but with your modifications, you can use this instead of Enclosure.obj.

