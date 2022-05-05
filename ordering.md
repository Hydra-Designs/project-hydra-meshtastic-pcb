# Ordering from JLCPCB


Download the Gerber-JLCPCB.{version}.zip file and the .zip file of the desired variant from the [Release](https://github.com/Hydra-Designs/project-hydra-meshtastic-pcb/releases/tag/2.1) and extract it to a local folder.
![image](https://user-images.githubusercontent.com/9000580/166714337-6639de76-8187-4cde-bb4a-ed1b411a9ce4.png)

Navgate to https://cart.jlcpcb.com/quote to start an order by uploading the gerber zip file.

![image](https://user-images.githubusercontent.com/9000580/166716300-16640bda-a35b-4ff1-94c4-c0c1b68091c5.png)

After the gerber file is loaded, select the quantity.

Enable the SMT Assembly section. Select "Assemble top side", choose a quantity, and for Tooling holes select "Added by Customer".
Click confirm to continue.
![image](https://user-images.githubusercontent.com/9000580/166716822-8628b8bd-1e19-4041-b34c-2e5437c6be81.png)

Upload the BoM-JLCPCB and CPL-JLCPCB .csv files from the unzipped variant directory and click next.
![image](https://user-images.githubusercontent.com/9000580/166718997-627a68b7-61df-4df7-a00d-424c53e3b047.png)

Review the parts list from the BoM and click Next. Manual changes to the BoM / CPL to swap equivalent parts out due to inventory shortages. 
Optionally, you can ignore these parts and source them from another vendor and manually solder them.
![image](https://user-images.githubusercontent.com/9000580/166719420-bc49029f-9603-487c-9bff-93c821e93de7.png)

Review the placement of the components from the CPL and hit Save to Cart.
![image](https://user-images.githubusercontent.com/9000580/166720516-6aa26568-ce6b-4a46-9441-195a0bf87de8.png)

After this process is complete, you can choose shipping and payment method at the checkout.
![image](https://user-images.githubusercontent.com/9000580/166720897-cf94f1c2-e3f6-4462-81f4-8e6a2f7338e9.png)


# Final assembly 

Ebyte E22-900M30S and ESP32-WROOM-32U modules as well as any out of stock parts will need to be purchased from LCSC or a preferred vendor. You will be responsible for [hand soldering](README.md#assembly-instructions) these components onto the board. Use the iBoM html file for component placement assistance.
