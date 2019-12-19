![DMX-Hue](dmxhue.png)

**OLA trigger config to control Philips Hue lights and Osram (LEDVANCE) Lightify products with DMX (Art-Net, sACN or via DMX input)**

[RGB version](https://github.com/gobo-ws/ola-trigger-rgb-hue-dmx)  

Lightify products works when paired with an Philips Hue bridge.

Should in theory also work with any other Zigbee Light Link (ZLL) or Zigbee 3.0 certified lamp that can be paired with an Philips Hue bridge.
For instance lamps from [Cree LED Connected](http://creebulb.com/connected), [GE Link](https://www.gelighting.com/led-bulbs/product-family-c-by-ge), [IKEA Trådfri](https://www.ikea.com/gb/en/products/lighting/smart-lighting), [Innr Lighting](https://www.innrlighting.com/en/), [Trust](https://www.trust.com/zigbee) etc.

There is only one lamp and one Lightify plug in this config but you can easy add more.    
Please note that the Hue bridge has some frame rate limits.  
SyntheFX has a good [article](https://support.synthe-fx.com/hc/en-us/articles/360034583252-Philips-Hue-Response-Times-vs-DMX) regarding Philips Hue response times vs. DMX.

Other things that can be added to this config is support for groups and so on.  
Check out the [Hue Developer site](https://developers.meethue.com) for more information.  
I have done some successful tests with scenes, but these are not officially published yet.

This config also works with the [deCONZ API](https://dresden-elektronik.github.io/deconz-rest-doc/) from Dresden Elektronik ([HuePass](https://github.com/KodeCR/hue-pass) or similar solution is needed for SSL support)

**Requirements**

* [OLA](https://www.openlighting.org/ola/)
* [curl](https://curl.haxx.se/)
* [Philips Hue bridge](https://www2.meethue.com) alternatively a gateway from [Dresden Elektronik](https://www.dresden-elektronik.de/funktechnik/solutions/wireless-light-control/gateways/?L=1)

**Installation**
  
* Download the [philips_hue_osram_lightify.conf](philips_hue_osram_lightify.conf) or [philips_hue_color_gamut_b.conf](philips_hue_color_gamut_b.conf) file and edit the configuration section.

[OLA trigger documentation](https://www.openlighting.org/ola/advanced-topics/ola-dmx-trigger/)

**Usage** 

* Before running ola_trigger, make sure that olad is running and the universe has been configured with a DMX512 source.  
The config file is provided on the command line:

`ola_trigger philips_hue_osram_lightify.conf`
