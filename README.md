**OLA Trigger config to control Philips Hue lights and Osram Lightify products with DMX (ArtNet, sACN or via DMX input)**

Osram Lightify products works when paired with an Philips Hue bridge.

Should in theory also work with any other Zigbee Light Link (ZLL) certified product that can be paired with an Philips Hue bridge. For instance Cree LED Connected, GE Link lamps ~~and the new smart lighting products (TRÅDFRI, JORMLIEN, SURTE & FLOALT) from IKEA~~

There is only one lamp and one Lightify plug in this config but you can easy add more.  Please note that the Hue bridge has some frame rate limits. SyntheFX has a good [article] (http://support.synthe-fx.com/customer/portal/articles/1330326-philips-hue-response-times-vs-dmx) regarding Philips Hue response times vs. DMX.

Other things that can be added to this config is support for groups and so on.  Check out the [Hue Developer site] (http://developers.meethue.com) for more information.

[OLA download] (https://www.openlighting.org/ola/)  
[OLA trigger documentation] (https://www.openlighting.org/ola/advanced-topics/ola-dmx-trigger/)

**Usage**  
Before running ola_trigger, make sure that olad is running and the universe has been configured with a DMX512 source.
The config file is provided on the command line:

`ola_trigger philips_hue_osram_lightify.conf`

/Johan Nilsson
