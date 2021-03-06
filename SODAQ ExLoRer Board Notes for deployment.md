# Software installation requirements and sources. 

#### Build and Deploy, Wuthering Bytes, 2017

## Microchip/SODAQ ExpLoRer Arduino installation

1. Install Arduino IDE    
2. Install board definition for SODAQ ExpLoRer    
	1. Menu File→Preferences
	2. Additional Boards URLs: Set to `http://downloads.sodaq.net/package_sodaq_samd_index.json`
	3. Click 'OK'
	4. Menu Tools→Boards→Boards Manager...
	5. Search for `SODAQ`
	6. Install `SODAQ SAMD Boards by SODAQ`

3. Install libraries
	1. Menu Sketch→Include Library→Manage Libraries...
	2. Search for `sodaq`. Click `install` button next to:
		* Sodaq_RN2483
		* Sodaq_wdt

4. Install Cayenne LPP libraries
	1. Menu Sketch→Include Library→Manage Libraries...
	2. Search for `cayenne`. Click `install` button next to:
		* CayenneLPP


Optional:

* Install RN4871 Bluetooth module    

	1. Download from http://support.sodaq.com/wp-content/uploads/2016/11/Microchip_RN487x.zip
	2. 	Menu Sketch→Include Library→Add .ZIP  Library...
	3. Browse to where `Microchip_RN2483x.zip` was downloaded and select it
	4. Click `Choose`

## Node-red

1. Install Node.js, if you don't already have it, from [nodejs.org/en/download/](https://nodejs.org/en/download/)

2. Install Node-red through the terminal      
```sudo npm install -g --unsafe-perm node-red```     
(via [nodered.org/docs/getting-started/installation.html](https://nodered.org/docs/getting-started/installation.html))

3. Run Node-red at the terminal    
```node-red```    
and (after a few moments) open a browser window with the url [127.0.0.1:1880/](http://127.0.0.1:1880/)

4. Terminate Node-red by pressing `CTRL`+`c` in the terminal window.