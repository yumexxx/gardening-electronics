<!-- to do:
	- consider reformatting so examples aren't mixed in w/ directions, is current format too confusing?
	- add pics for better engagement
	- add code examples
	- is it ok that this is dually a guide and documentation of example? I think that kids can be creative/have freedom with this project and I don't want to limit them with just our example
-->


# Water Level Sensor :droplet:
**Goal:** Let's use micro:bit's built in **accelerometer** to monitor the amount of water in a hydroponics system!

<!-- insert diagram showing accelerometer on micro:bit -->

You have **lots of freedom** to construct your apparatus and design your code as you wish, keeping in mind the goal to detect amount of water in your system. Feel free to follow the example below, improve upon it, and/or create your own design!

![GIF of water level sensor rising with water](https://github.com/yumexxx/gardening-electronics/blob/main/water%20level%20sensor/water%20level%20rising.GIF.gif)

### Materials
#### Electronics :battery:
- [ ] (1) micro:bit (with USB cord)
- [ ] (1) battery pack (for AA batteries) with connector
- [ ] (2) AA batteries
#### Craft Materials (see sub-bullets for example choices!) :art:
- [ ] a base & frame for micro:bit and physical water sensor
	- (2) 1/2"-thick, 1 ft. long wooden rods (we cut these from one longer rod)
	- (1) 1" thick long wooden block
- [ ] fasteners/something to connect parts considering desired movement (stability, rotation, etc.)
	- (2) long wood screws
	- (2) thin wooden skewers
- [ ] something to sense movement of water
	- (1) block of styrofoam (look around for packages with this!)
- [ ] something to hold the micro:bit, safe from water
	- scrap cardboard
	- tape

### Tools :toolbox:
- [ ] MakeCode for micro:bit (online block/Python coding software)
- [ ] drill (Phillips & woodboring bits for wood screws and holes)
- [ ] saw
- [ ] clamps (to secure wood while cutting/drilling)
- [ ] box cutter / scissors
- [ ] marker (to mark measurements/align parts)
- [ ] ruler (to fit apparatus to dimensions of hydroponics system)

## Let's make it! :triangular_ruler:
### Plan the Design :pencil:
**Make a rough plan & sketch of your apparatus**
- will your structure be freestanding? attached to the hydroponics container?
- how will you translate a physical sensor of water level to be detected as changing velocity/position by the micro:bit?
- what materials do you have available already to build a stable & durable structure and design a water level sensor? what other materials can you easily get?

	Example:
	- with a small & light container, we chose to make the structure freestanding to ensure stability of the sensor over time without affecting the stability of the hydroponics system
	- stick a styrofoam block at one end of a skewer to sit in water, and attach the micro:bit at the other end of the skewer on a free-rotating piece of cardboard, so when the styrofoam floats on the surface of the water as its height changes, the micro:bit tilts up or down
	- materials:
		- we had a wood scrap bin, so decided to build the frame and base out of wood (using rods, skewers, and blocks)
		- we chose cardboard to attach the micro:bit to since it is easy to cut & prototype quickly with (and we had plenty lying around)
		- looking for a durable & buoyant material that would float on the surface of the water as its height changed, we found styrofoam from old packaging to cut into smaller chunks

### Plan the Code :computer:
Play around with the accelerometer blocks (including tilt!) and simulator in MakeCode to see how accelerometer readings (based on changing velocity/position) can be translated into a user-friendly output showing 'water level.' Consider using variables to save different readings. Also try out the many built in features (LED display, buttons, golden touch sensors) to allow user interaction with the micro:bit to read _multiple_ pieces of information, if desired.
1. Start by showing the number of different readings on the LED display
2. Choose a reading that, based on your physical design, shows the changing water level
3. Determine an appropriate & user friendly scale to output the 'water level' (search for the 'map' function to scale the default readings to a customized scale)
4. Graph the reading, and play with other ways of displaying the water level reading.
5. Saving all your work as a .hex file from MakeCode, choose your favorite method of translating water level to display. Finalize a rough draft of the code, so that it works as you expect with the simulator, and is ready to be tested after you make the physical apparatus.
**It is important to start thinking about how your program will connect the physical and digital worlds to ultimately monitor water level before starting the physical build, in case any adjustments to your physical design are needed based on what you can do with MakeCode**

	Example:
	![micro:bit water level sensor code](https://github.com/yumexxx/gardening-electronics/blob/main/water%20level%20sensor/microbit%20code%20w%20buttons%20for%20graph%20and%20number.png)

### Measure & Mark :straight_ruler:
**Plan your dimensions and measure & mark materials**
- how tall and wide is your hydroponics system? how do you want your water level sensor positioned relative to the system (i.e. how far should the micro:bit be above to detect significant water level changes?)
- how wide do you want your base to be to ensure a space-efficient & stable structure?

	Example:
	- the black bin pictured above is 10 inches wide and 8 inches tall
		- we wanted the micro:bit 6 inches above the top of the black container when the micro:bit is flat (parallel to the water surface), making the length between the micro:bit and styrofoam about 7 inches, so that the micro:bit and cardboard it's attached to have enough space to rotate down to be completely vertical (if the water level is extremely low)
	- we made our base 8 inches wide (slightly smaller than the width of the container), which seemed wide enough for stability, but did not take up much extra space outside of the system
	- we measured and marked:
		- desired length of wooden base as 8" (original block was longer and took up more space than desired)
		- location on base to perpendicularly attach wooden rods (rods 4 inches apart, each two inches from the center of the base and edge on either side), marked location where center of circular cross section of rod meets the base to drill hole & screw later on (on **both** the top and bottom of the block for later attachments)
		- height along rods to drill holes to put free-spinning skewer through as 10" from bottom end at the base and in the center of the rod's width (so micro:bit can tilt based on the height of the water)
		- size of cardboard to house micro:bit (3.5" wide to fit within the wooden rods, and 5" long to allow skewer & styrofoam flexible range of motion for a wide range of possible water heights)
		- area on cardboard to later cut out an indent for the micro:bit to rest in (and get taped in for extra security!)
		- point near long end of cardboard to later stick skewer for styrofoam through
		- length of sides of the styrofoam block (1.5" each side), so the block would be large enough to reliably float at the water's surface over time, but small enough to take up little space in the water of the hydroponics system, and fit through one of the plant-cup holes (not pictured, about the size of the top of the red cup) in the bin lid so the block could rise with the water as needed, and be easily removed for repair & maintenance of the water level sensor

### Let's Build! :screwdriver:
_the following steps are specific to the example design, read along for building & safety tips!_
1. Cut wooden parts with saw to measured marks (base, two rods).
- **make sure to secure wood safely with clamps, and as for help if needed!**
2. To drill the holes for the skewer through each rod, one at a time, secure both ends of a rod to a clean & sturdy woodworking surface with clamps, making sure to have either a gap under the area where the hole will be drilled, or a scrapable & thick wooden surface underneath. Using a hole-boring bit, drill the hold in the marked location.
3. Still using the hole-boring bit, face the designated bottom of the base upwards, and on each of the two marked locations for the rods, drill an indent halfway through the thickness of the base (to prepare the area to drill the screws in)
4. Switch. the drill bit to a Phillips bit. To attach each of the rods to the base, ask a friend to help hold/secure the rod in its designated location against the base, making sure that the pre-drilled holes for the skewer near the top ends of each rod are running along the length of the base (don't fret, the rods can be twisted a little for fine adjustments once they're screwed into the base).
5. Facing the bottom of the base with a wood screw magnetically attached to the drill bit, position the screw over the pre-drilled indent and drill the screw in until the rod is secured against the base. Repeat for the second rod.
6. Place the base and rods upright on working surface and put one skewer through the holes near the top of the rods.
7. Using a box cutter or scissors, cut cardboard to measured size, and lightly trace the indent area for the micro:bit with a blade. With the blade covered and on the table, use your fingers (or a pen) to lift and remove the top layer of cardboard for the micro:bit area.
8. Tape the short end of the cardboard (making sure it's the short end _without_ the mark for a hole) along the skewer between the rods.
9. With the pointy end of the second skewer, poke a hole through the designated mark, and push the skewer through until at least 7" of the skewer is below the cardboard. Stick the styrofoam block into the middle of this second skewer.

**Last step before testing!** Download your rough draft code onto the micro:bit, attach the battery pack (not pictured), and securely tape the micro:bit and battery pack onto the cardboard.

### Test and prototype!
Run the code on your micro:bit to see how your program works along with your physical structure.
**Do not worry if your plan doesn't function as you expected right away, it is important to embrace the testing & prototyping process.**
_Right now, see..._
- how does your device 'react' when you manually change the water level (try pouring in more water to a small cup or bowl)?
- does the micro:bit display data as you expected?
- how can you consider the micro:bit's energy use in your program design? consider how often you display data, whether it be automatically or in reaction to user interaction
_...over time, observe_
- how does your structure hold up in the environment? does it fit into the workflow of your garden?
- how reliable is the micro:bit water level display?
- can you access the data/display easily and quickly? are you provided too little, too much, or just enough data?

#### Nice job! You did it :). As you incorporate a water level sensor into your garden, you will see over time what features work, and what features can be improved to fit in with the garden as it evolves.
Based on where your interests lie, feel free to let this sensor run on its own and interact how you've designed, observing occasionally for any desired adjustments, or try out some of the extensions on this project below.


### Possible Extensions :)
- connect this system to an automatic pump (see micro:bit soil moisture tutorial **to be updated soon** with pump guide) to automatically pump water into the system as needed (you determine when that is based on the data you get!)
- log water level data over time to track the well-being of your hydroponics system, and consider track the level for different plants/set-ups to learn how water is consumed at different rates based on different plant configurations
- (if micro:bit V2 is available) use two micro:bits and the radio feature to send data from one micro:bit (the sensor, attached to the cardboard) to a second micro:bit (the receiver & displayer, to show the water level as a number, graph, etc.)
- so much more -- play around and have fun!