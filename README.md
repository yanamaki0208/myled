# myled

This illuminates the LEDs on pins 23, 24, and 25.

# DEMO
![スクリーンショット (207)](https://user-images.githubusercontent.com/66021066/101283347-15730a80-381d-11eb-900f-b3c516a028a8.png)

# Usage

*copy the repository  
`git clone https://github.com/yanamaki0208/myled.git`  

*move directory  
`cd myled`  

*compile "myled.c"  
`make`  

*install the module  
`sudo insmod myled.ko`  

*change permissions  
`sudo chmod 666 /dev/myled0`    


*turn off the red LED  
`echo 0 < /dev/myled0`  

*turn off the yellow LED  
`echo 1 < /dev/myled0`

*turn off the blue LED  
`echo 2 < /dev/myled0`  

*turn off all LEDs  
`echo 012 < /dev/myled0`    


*turn on the red LED  
`echo 3 < /dev/myled0`  

*turn on the yellow LED  
`echo 4 < /dev/myled0`  

*turn on the blue LED  
`echo 5 < /dev/myled0`

*turn on all LEDs  
`echo 345 < /dev/myled0`  

*uninstall the module   
`sudo rmmod meled.ko`  

# Note
Connect the anode to GPIO pin and the cathode to ground.

# Author

* Masaki Yara and Ryuichi Ueda  
* Chiba Institute of Technology  
* masaki.yara@gmail.com  

# License

"myled" is under [GNU General Public License v3.0](https://ja.wikipedia.org/wiki/GNU_General_Public_License#%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B33).
