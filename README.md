# Yamaha RXS100 Electrics!

There are very limited resources available regarding this model, so I thought I'd do some experiments and research and publish my findings for all to use. I will document the following goals:

My first goal is to publish a new and complete, checked wiring diagram of the RXS100. 
My second goal is to explain exactly how the wiring works.
My third goal is to propose a solution to a 10.8-12.6v lithium conversion.
My fourth goal is to convert it!

As I work on the project, I aim to release schematics and videos. The schematics can be viewing in this repo, but the videos will be shown below:

STATOR: https://www.youtube.com/watch?v=sNIP0P2Dm8Q&lc=UgxLB3ARer4_yUKb1mJ4AaABAg.9x9-UrGFVLW9x91tnFPku4


NEW RX100 THUMBSWITCH MOD: https://www.youtube.com/watch?v=C9AQ84TwCFk

HOW THE RXS100 ELECTRICS WORK:

The RXS100 has two power sources; A generator and a battery.
*From the battery: (DC power)*
Battery current goes from anode through a fuse to the ignition switch via red wire (also to the rectifier, but it cannot pass through it). If the ignition is on then the red wire is linked to the light brown wire.
The light brown wire allows current to flow to the following;
The front and rear brake light switch (they're wired in parallel - high side switches) - Current flows through the yellow and green wire to the stop/tail lamp in the rear light assembly, then through to ground.
The flasher relay - This is switched low side, comes through brown and white wire to the indicator switch. Depending on position, current flows through dark green or dark brown through the lamps then to ground.
The horn - Current flows through the horn through pink wire to the switch, then to ground.
The oil and neutral lights - These are switched low side. The oil light is a black and red wire and it goes to the oil level switch (something strange is happening here which I've not yet worked out). The neutral wire is soft blue. This wire goes to the oil level switch and the generator according to the wiring diagram. This doesn't make sense and I haven't validated it yet. The diagram makes no mention of the neutral switch. However, on my bike, when the neutral switch is pressed by the gear box, the light comes on whether on ignition or running. The oil switch is a stange one. If the engine is off, but ignition is on AND you're in neutral, the oil lamp glows. God knows how- I haven't worked it out yet.
What one can ascertain so far is that all components listed above are battery powered. Although the oil/neutral wires need checking.
*From the generator: (AC power)*
The stator has three coils in it. As the engine rotates the magnet around the coils, a voltage is made. One coil appears to be a pulser coil, another lighting coil and another charging coil.
The pulser coil has a red and white wire. This goes to the CDI unit and probably pulses the ignition coil, which in turn sends a high voltage across the spark plug.
There's a black and red wire which comes from the generator also. I'm thinking that this wire powers the CDI itself. It also appears to go to the igintion switch. I'm thinking that this gets shorted to the black wire (ground) when the ignition is off. What this would mean is that the CDI won't operate unless someone has the key, also when you switch off, any power generated the last second would be dead-shorted instead of powering the CDI for another spark.
The soft blue wire - I'm not sure what it does yet, but it's something to do with the oil light... ? It's probably used as a signalling wire. If this wire has voltage then only show oil when switch is activated, otherwise show the oil light if it's also in neutral. I don't know. Something like that.
The green and red wire - This is the charging wire/coil. This goes to the rectifier which only lets a positive voltage through. In other words, any negatively charged power gets lost. That's not a great design as half of the power generated is wasted. Why? Anyway, from the rectifier, the then DC voltage then goes to the battery anode to charge it up. If the lighting switch is off, then additionally, the high side gets connected to the voltage regulator (which is maybe a zener diode), which burns off excess voltage whilst charging the battery.
The yellow and red wire - This is the lighing power wire. It goes to the lighing switch. If the lights are off, this is an open circuit and nothing more happens with this wire. If it's on, this power is connected to blue and white? (maybe red), and yellow and white. Yellow and white is the regulator which burns off excessive voltage so that the bulbs don't blow. Blue and red however, powers the instrument cluster which go straight to ground. Additionally, it powers the auxilliary lamp. If you have lights on full, not PO, then either the headlamp gets power OR the high beam along with the high beam indicator bulb.
