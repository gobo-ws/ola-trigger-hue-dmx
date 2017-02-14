**OLA Trigger config to control Philips Hue lights and Osram (LEDVANCE) Lightify products with DMX (ArtNet, sACN or via DMX input)**

Lightify products works when paired with an Philips Hue bridge.

Should in theory also work with any other Zigbee Light Link (ZLL) certified product that can be paired with an Philips Hue bridge.
For instance lamps from [Innr Lighting] (http://www.innrlighting.com), [Cree LED Connected] (http://creebulb.com/connected), [GE Link] (http://www.gelinkbulbs.com/) etc.

There is only one lamp and one Lightify plug in this config but you can easy add more.    
Please note that the Hue bridge has some frame rate limits.  
SyntheFX has a good [article] (http://support.synthe-fx.com/customer/portal/articles/1330326-philips-hue-response-times-vs-dmx) regarding Philips Hue response times vs. DMX.

Other things that can be added to this config is support for groups and so on.  
Check out the [Hue Developer site] (http://developers.meethue.com) for more information.

**Requirements**

* [OLA] (https://www.openlighting.org/ola/)
* [curl] (https://curl.haxx.se/)
* [Philips Hue bridge] (http://www2.meethue.com)

**Installation**
  
* Download the [philips_hue_osram_lightify.conf] (philips_hue_osram_lightify.conf) or [philips_hue_color_gamut_b.conf] (philips_hue_color_gamut_b.conf) file and edit the configuration section.

[OLA trigger documentation] (https://www.openlighting.org/ola/advanced-topics/ola-dmx-trigger/)

**Usage** 

* Before running ola_trigger, make sure that olad is running and the universe has been configured with a DMX512 source.  
The config file is provided on the command line:

`ola_trigger philips_hue_osram_lightify.conf`
