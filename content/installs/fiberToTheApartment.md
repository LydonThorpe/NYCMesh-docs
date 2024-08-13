---
title: "Fiber to the apartment"
aliases: ["/fiber"]
---

The first step is to screw the ONT into the wall in a convenient place using drywall achors. The ONT we are currently using is the Ubiquiti UF-WiFi6-US

Only use white fiber inside apartments, never yellow or any other color. This is to better blend in with the wall. We have custom made 3mm white fiber with termination at one end. 

Once the ONT is screwed into the wall, plug in the terminated end of the white fiber. Now you are ready to run the fiber to the exit point (usually above the front door). You first run the fiber down to the top of the baseboard and then along to the nearest corner, attaching it to the wall with silicone or staples. You run the cable up the corner to the ceiling and follow along the corner of the ceiling to the exit point using silicone or staples along the way.

![Ufiber ONT](/img/installs/wallONT.jpg)

As always with fiber, don't do any hard bends! Let the fiber curve around corners.

There is no loose fiber in the apartment, just a service loop above the door. All the fiber is locked down with silicone or staples the whole way. Any loose fiber will result in service calls. Excess fiber is pulled back into the apartment and left as a service loop above the door. Trim the yellow raceway fiber down before splicing so it one foot from the entry point. Use excess white fiber to enable the splice.

At the exit point you drill a small hole (6mm?) and feed the unterminated end of the fiber through to the raceway. The fiber will be spliced outside of the apartment either with a fusion splicer or with a mechanical splice. The hole must be sealed after you're finished!

The new ONT has a built in router so install it near a power outlet and you are done. You will need to log into the OLT to configure the router

The older model ONT is powered by connecting it to a POE injector, and connecting the data port to a TP-Link/Archer home router. 

**Support**

[to be expanded!]

Fiber support is fairly straightforward. First do the usual test of the wifi router to eliminate that as the problem. Next test the signal going into the ONT by unplugging the connector and connecting it to your meter.

Test db of signal using an OTDR or optical power meter (OPM). The signal should be between -22db to -10db. Less than -24db and the signal is too weak. -8db is the highest limit that will work. 

If the signal is outside of the range of -22 to -10 you need to look for where signal loss is occurring. This is typically the splice in the raceway or damaged fiber that has been bent.

Light fiber with red test signal using the OPM or OTDR. This is done from the hallway access box.

Look for loss along the way, especially in the raceway splice. Redo splice if signal loss is there. If the cable is damaged elsewhere, splice around the damage.
