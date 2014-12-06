#BrewPi build with parts in North America
The BrewPi as listed below is no longer available. It appears that they have a new product release coming out based on the Spark Core.  Elco, \_mdma, and Geo have done an excellent job with BrewPi so support them when you can. However, for those of us on a budget and in North Amercia it is a little pricey and takes a while when purchasing from them. We've written up the BrewPi build with parts that can be 95% sourced from Amazon and the price is around ~120. You could go cheaper if you have some of the stuff around the house. 

I followed a very similar guide to build mine. [The guide I used was provided by Homebrewtalk user FuzzeWuzze](http://www.homebrewtalk.com/f258/howto-make-brewpi-fermentation-controller-cheap-466106/). I've made a few changes to this guide as well as wanted an open source and forkable guide for improvements. 

- Cost ~$120 USD
- Time ~2 hours

### Parts List

- [RaspberryPi Kit](http://www.amazon.com/gp/product/B008XVAVAW/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1) (This is the biggest cost at $60. You can go cheaper if you have an old computer laying around that you aren’t using. Just install the same linux distro and BAM. You can also go cheaper if you have the SD card and power cord around and only have the buy the Raspberry Pi board)
- [Adruino UNO](http://www.amazon.com/gp/product/B00E5WJSHK/ref=oh_aui_detailpage_o02_s01?ie=UTF8&psc=1) This one is made by SainSmart. Has solid reviews and cheaper than the other brands. There are even cheaper if you don’t mind waiting from China.
- [2 Channel Relay](http://www.amazon.com/gp/product/B0057OC6D8/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1) - I like this one. But as long as it has 120 volt and 10A capacity, you should be good.
- [DS18B20 Temp sensors](http://www.amazon.com/gp/product/B00M2S564I/ref=oh_aui_detailpage_o02_s01?ie=UTF8&psc=1) - Any of these will work. You’ll want water proof just in case (even though you’re using a themowell). Also you’ll want to make sure the ones you order will be small enough for your thermowell. 6 mm is a good size to shoot for. *Note: The temp sensors linked needed to be extended for my build. Also, the rubber sheathing on the SS needed to be shaved off to fit in the linked thermowell.*
- [Power cord](http://www.amazon.com/gp/product/B002O0KM6G/ref=oh_aui_detailpage_o02_s00?ie=UTF8&psc=1)- (You could go cheaper and repurpose and old extension cord or old power cord from something else that’s junk.)
- [Terminal Strip](http://www.amazon.com/gp/product/B005I03WOI/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1) - (easier and cleaner than wire nuts but you could use those if you’re going on the cheap)
- [Wall socket](http://www.amazon.com/gp/product/B0012DRL4C/ref=oh_aui_detailpage_o02_s02?ie=UTF8&psc=1) - (You could easily purchase something at home depot or find one at home)
- [12 gauge wire](http://www.amazon.com/gp/product/B00INVF486/ref=oh_aui_detailpage_o02_s02?ie=UTF8&psc=1) - Again, you could find this anywhere. I recommend making sure you have proper colours so you don’t confuse your hot/neutral/ground
- Wire nuts

### Tools 

- Wire cutters
- Wire strippers
- Phillip screwdriver
- Flathead screwdriver
- Solder gun - Not necessary if you have the right connectors for the pins, but I found it useful because I didn't have the right connectors. 

### Wiring Schematic

I have used the schematic below that was provided by 100Amps on Homebrewtalk.com. 

![](https://github.com/open-homebrewing-project/home-brewing-automation/blob/feature/fermentation/images/brewpi-wiring-schematic.gif) 

The Sainsmart relay board does have male pins instead of female. If they were female then it would be easy to use jumper cables or wires to insert. Since they are male, it appears some people have pulled the header pins out and solder the wires to the pads as FuzzeWuzze mentions in his guide. I did something similar, however, soldered directly to the male pins. This was a pain in the ass and I highly recommend pulling the header pins out unless you're as stubborn as I. 

You'll want to wire everything up before connecting to a live power source. I think this is fairly obvious. 

### Installation  
