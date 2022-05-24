# Temperature, Humidity and CO2 Sensor
Steps to connect the Sensirion I2C SCD41 Temperature & Humidity sensor using Arduino IDE

# Software Setup
1. Download Arduino IDE here 
(under Downloads -> Download options -> select operating system)
Follow download prompts for IDE until a window similar to the one below opens
![alt text](https://user-images.githubusercontent.com/95435534/164768973-afcd56a4-de3f-4a5a-8b17-330372a2d3c0.png)
2. Download the Sensirion Library
(under Code -> Download ZIP)
Move the downloaded ZIP folder to an accessible location (i.e. Desktop)
Import the Sensirion Library
Open Arduino IDE
Navigate to Sketch - > Include Library -> Add .ZIP Library… 
![alt text](https://user-images.githubusercontent.com/95435534/164768979-5aa19c11-6bc0-4fcc-9417-2b60bff3951d.png)
Select the ZIP folder from the saved location in step 2a
Once you have uploaded the folder, navigate to File -> Examples and verify that Sensirion examples are displayed (at the bottom of the list)
![alt text](https://user-images.githubusercontent.com/95435534/164768997-1766068e-51d0-45c9-969f-84d5f52bf27b.png)

# Physical Setup
Setup Grove - CO2 & Temperature & Humanity Sensor (SCD41)
1. Unbox R2040
![alt text](https://user-images.githubusercontent.com/95435534/164769009-9ea1b07d-1681-41ad-b46d-0e992fb58e65.png)

2. If Using Grove Shield:
Clip or bend reset pins (RST) on either side 
![alt text](https://user-images.githubusercontent.com/95435534/164769021-02942ce5-efd0-4e0e-b4b7-8fbf524231cd.png)

Line up pins with labels on shield
![alt text](https://user-images.githubusercontent.com/95435534/164769024-e20d591f-ef97-43ae-a3cb-08047cea3fa1.png)
Snap pins into place
![alt text](https://user-images.githubusercontent.com/95435534/164769031-e24ae10d-19b1-4ba1-8b1f-a5929fa2ee62.png)

3. Remove the SCD41 sensor from its packaging

4. Locate the I2C port on the shield 

5. Connect the SCD41 sensor cord to the I2C port of the shield

6. For wired connection:
Use a micro USB cable plugged into a powersource (laptop, desktop, etc.)
Attach the micro USB to the arduino as shown
Note: A green LED should appear indicating it is powered on

Navigate to Tools -> Board: and verify that “Arduino Nano RP2040 Connect” is selected
Now navigate to Tools -> Port -> /dev/cu.usbmodemxxxx (Arduino Nano RP2040 Connect) 
Note: This may look a little different depending on the port and device used

7. Open the Arduino IDE on your interface
8. Navigate to File -> Examples -> Sensirion I2C SCD4x -> exampleUsage
Note: The file should look like the one below


9. Navigate to Tools -> Serial Monitor
Note: A blank window should open with this command. This is where you will view the printout statements from your code.

10. Run the code by clicking the “upload” button

Refer to the serial monitor window. It should look something like below
Note: Notice that the values update every 5 seconds


11. Teardown:
Close the serial monitor 
Quit Arduino IDE
Disconnect arduino from power source
Disconnect sensor from port and store

