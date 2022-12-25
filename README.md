# 1541-II-1581-power-distribution-pcb

Allows up to four 4-pin DIN Commodore Floppy Disk Drives to use a single Power Supply

![IMG_20221224_080939-1920](https://user-images.githubusercontent.com/9030553/209482304-8f4bd88b-01ae-430a-8a50-154f14c88ff4.jpg)

I created this PCB to eliminate the growing pile of power supplies needed to
power my stack of Commodore Floppy Disk Drives. Feeing up three AC power outlets is
also a bonus!

I have not specified any particular enclosure as what suits me may not be ideal 
in your situation. I'm happy to metal enclosures but some prefer plastic.

Mouser
490-SDS-40J - x4 SDS-40J 4-Pin DIN
576-04450001N - x4 Fuse Clip PCB
490-TB006-508-04BE - x1 4-Way Terminal Block 5.08mm

Digikey
CP-2340-ND - x4 SDS-40J 4-Pin DIN
F6083-ND - x4 Fuse Clip PCB
102-6193-ND - x1 4 Way Terminal Block 5.08mm

For the optional Power LED header, resistors and LEDs/cabling, any convenient 
parts can be used so I've not specified exact part numbers. The PCB pads suit
0805 size SMD resistors.

R1 300R 0805 (2012 metric) (5V Rail)
R2 1K 0805 (2012 metric) (12V Rail)
3 Way 2.54mm header

I like using the metal cased DIN plugs but feel free to use whatever you can source. The 
Switchcraft DIN plugs are quite expensive compared to those with plastic covers.

Digikey
SC1607-ND - Switchcraft 4-Pin DIN Plug

Mouser
502-09BL4MX - Switchcraft 4-Pin DIN Plug 

RS has their own branded metal cased DIN plugs that both look quite good and are cheaper 
than the Switchcraft DIN plugs.

491-134 RS PRO 4 Pole Din Plug, 1A, 100 V ac, Male, Cable Mount

BShorter cables from the distribtion board to the floppy drives will give you less voltage 
drop. The 5V output on the RD-65A can be set slightly higher to allow for this.

To connect to a 1541-II or 1581 you need to make 1 to 1 cables with three core cable.
I used 0.75mm cable that is commonly used for AC Mains appliances here in Australia.

Pin 1 - 5V
Pin 2 - GND
Pin 3 - N/C
Pin 4 - 12V

I used a MeanWell RD-65A Power supply but you can use any 12V/5V Power Supply that can 
supply at least 5V at 4A and 12V at 4A. Commodore 1581 Drives do not need 12V and if you
only use 1581 drives you can get away with using a single 5V Power Supply with sufficent
current capacity.

Mouser
709-RD65A - x1 RD-65A Meanwell Power Supply

Digikey
1866-3987-ND - x1 RD-65A Meanwell Power Supply
