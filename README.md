Radio controlled arduino quadcopter project

This is very simple arduino quadcopter project. It's still far from finished, but it does kind of work.

I recommend opening this with Arduinio IDE 1.0.5 or later

1) Parts which are required to run this project:

	* Any arduino
	* MPU-6050
	* RC receiver and transmitter
	* 4 motors
	* 4 ESC's
	* A battery
	* And a frame, of course

2) How to connect MPU-6050 to your arduino?


Connect them according to this table:

        Board                   |        I2C / TWI pins
        -------------------------------------------------
        *Uno, Ethernet          |        A4 (SDA), A5 (SCL)
        *Pro mini               |        A4 (SDA), A5 (SCL)
        *Mega2560               |        20 (SDA), 21 (SCL)
        *Leonardo               |        2 (SDA), 3 (SCL)
        *Due                    |        20 (SDA), 21 (SCL), SDA1, SCL1

Also, you will have to connect INT pin from MPU-6050 to 2nd pin on UNO, Pro mini, DUE, Ethernet and Mega2560.
If you are using Leonardo then connect it to the 3rd pin.

3) How to start logging data from your quadcopter:

	1) Compile and run logger located in Processing/src using Processing IDE
	2) Disconnect any unnecessary USB devices connected to your computer (mobile phones, tablets, mp3 players etc)
	3) Connect your quadcopter arduino through USB to Serial cable to your computer
	4) Wait few seconds, and you should

At this point my logging software is unfinished and is barely useful. I just wanted to quick way so see some data, and I have plans to improve it.
If anyone is interested in making it more appealing, adding more features and making it overall more useful, please be free to do so.
Contact me if you have added some new features, I could update this repository with your code so everyone could use it.

Some info on how RC channels, controller and ESC's are interlocked:
![alt tag](http://s30.postimg.org/cx98h86kh/2014_10_16_18_33_12.jpg)

Some videos showing how my quadcopter functions using this code:

https://www.youtube.com/watch?v=enUAQP_ES2M

https://www.youtube.com/watch?v=QN5GNv5YQQ0&list=UUeCGTW1pIbjfbPbLZzreOzQ


You can contact me at EdvinasKilbauskas@gmail.com or at github http://github.com/EdvinasKilbauskas
