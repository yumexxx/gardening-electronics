# Temperature, Humidity and CO2 Sensor
Steps to connect the Sensirion I2C SCD41 Temperature & Humidity sensor using Arduino IDE

Software Setup
#1. Download Arduino IDE here 
(under Downloads -> Download options -> select operating system)
Follow download prompts for IDE until a window similar to the one on the right opens 
Download the Sensirion Library here 
(under Code -> Download ZIP)
Move the downloaded ZIP folder to an accessible location (i.e. Desktop)
Import the Sensirion Library
Open Arduino IDE
Navigate to Sketch - > Include Library -> Add .ZIP Library… 
Select the ZIP folder from the saved location in step 2a
Once you have uploaded the folder, navigate to File -> Examples and verify that Sensirion examples are displayed (at the bottom of the list)


Physical Setup
Setup Grove - CO2 & Temperature & Humanity Sensor (SCD41)
Unbox R2040


If Using Grove Shield:
Clip or bend reset pins (RST) on either side 


Line up pins with labels on shield

Snap pins into place


Remove the SCD41 sensor from its packaging

Locate the I2C port on the shield 

Connect the SCD41 sensor cord to the I2C port of the shield

For wired connection:
Use a micro USB cable plugged into a powersource (laptop, desktop, etc.)
Attach the micro USB to the arduino as shown
Note: A green LED should appear indicating it is powered on

Navigate to Tools -> Board: and verify that “Arduino Nano RP2040 Connect” is selected
Now navigate to Tools -> Port -> /dev/cu.usbmodemxxxx (Arduino Nano RP2040 Connect) 
Note: This may look a little different depending on the port and device used

Open the Arduino IDE on your interface
Navigate to File -> Examples -> Sensirion I2C SCD4x -> exampleUsage
Note: The file should look like the one below


Navigate to Tools -> Serial Monitor
Note: A blank window should open with this command. This is where you will view the printout statements from your code.

Run the code by clicking the “upload” button

Refer to the serial monitor window. It should look something like below
Note: Notice that the values update every 5 seconds


Teardown:
Close the serial monitor 
Quit Arduino IDE
Disconnect arduino from power source
Disconnect sensor from port and store

