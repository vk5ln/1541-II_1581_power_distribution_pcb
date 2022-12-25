# 1541-II-1581-power-distribution-pcb

Allows up to four 4-pin DIN Commodore Floppy Disk Drives to use a single Power Supply

![IMG_20221224_080939-1920](https://user-images.githubusercontent.com/9030553/209482304-8f4bd88b-01ae-430a-8a50-154f14c88ff4.jpg)

I created this PCB to eliminate the growing pile of power supplies needed to
power my stack of Commodore Floppy Disk Drives. Feeing up three AC power outlets is
also a bonus!

I have not specified any particular enclosure as what suits me may not be ideal 
in your situation. I'm happy to metal enclosures but some prefer plastic.

For the optional Power LED header, resistors and LEDs/cabling, any convenient 
parts can be used so I've not specified exact part numbers. The PCB pads suit
0805 size SMD resistors.

R1 300R 0805 (2012 metric)
R2 1K 0805 (2012 metric)
3 Way 2.54mm header

I like using the metal cased DIN plugs but feel free to use whatever you can source. The 
Switchcraft DIN plugs are quite expensive compared to those with plastic covers.

RS has their own branded metal cased DIN plugs that both look quite good and are cheaper 
than the Switchcraft DIN plugs.

Shorter cables from the distribtion board to the floppy drives will give you less voltage 
drop. The 5V output on the RD-65A can be set slightly higher to compensate for this.

To connect to a 1541-II or 1581 you need to make 1 to 1 cables with three core cable.
I used 0.75mm cable that is commonly used for AC Mains appliances here in Australia.

Pin 1 - 5V
Pin 2 - GND
Pin 3 - N/C
Pin 4 - 12V

My Excellerator+PLus drive has a 5-Pin DIN socket for power input so I made one cable with
a 4-Pin DIN on one end and a 5-Pin DIN on the other. This plug has been marked to make sure
it doesn't get connected to anything else! I would hate to think what would happen if it were
to get plugged into a Commodore 64 power socket or worse, the AV output socket! 

I used a MeanWell RD-65A Power supply but you can use any 12V/5V Power Supply that can 
supply at least 5V at 4A and 12V at 4A. Commodore 1581 Drives do not need 12V and if you
only use 1581 drives you can get away with using a single 5V Power Supply with sufficent
current capacity. A surplus ATX power supply could be used, this has the advantage of the AC
input of the power supply being safely inside an exiting metal enclosure. 

The MeanWell RD-65A has AC input terminals which are exposed and can be accessed by curious fingers. 
It is intended to be used within another enclosure. The photos I show of my test setup sitting on a desk 
is NOT a recommended permanent solution. 

The 5V and 12V fuse values can be varied to suit your set up. While designing the PCB I sat down and 
measured the current consumption on each of my floppy disk drives.

1541-II 
12V - Idle 0.04A - Active 0.400A
5V - Idle 0.42A - Active 0.44A

1581
12V - Idle 0.00A - Active 0.00A (it doesn't use 12V at all)
5V - Idle 0.36A  - Active 0.63A

Excelerator+Plus
12V - Idle 0.29A - Active 0.36A
5V - Idle 0.56A - Active 0.56A

If I was reading/writing from all four drives at once (which is unlikely) I need a maximum of 1.16A @12V and just over 2A @ 5V... well within what a Meanwell RD-65A can handle.

