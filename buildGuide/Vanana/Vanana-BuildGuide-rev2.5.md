

# Vanana (rev 2.5 GB) Build Guide

Last Update: 210520

We will go through the process of fully assembling Vanana as shown in the photo below:

![2-d3](Vanana-BuildGuide-rev2.5.assets/2-d3.jpeg)

## Required parts:

![0-prep](Vanana-BuildGuide-rev2.5.assets/0-prep-1621563771641.jpg)

**Essential hardware used to make this build:** 

- Vanana Thicc Case x 1  
- Vanana white Plate x 1 
- m2 screws 7mm x 4
- m2 screws 18mm x 10 
- m2 Standoff 5mm x 10 
- m2 Standoff 4mm x 10 
- m2 Nuts x 10 
- m2 Washer x 10  
- EC11 Rotary Encoder x 1 
- Dupont cable x 3 
- Right angle headers
- Straight angle headers (This usually comes with your MCU. Make sure that the height of the insulation is less than or equal to 3mm)

**Optional hardware for a wireless build:** 

- Dupont cable x 6 (2 cables for RGB, Power switches and battery) 
- Slide Switch x 2
- LiPo Battery  **(will not be included in the GB kits)**

**Optional hardware for a Hot-swap functionality:** 

- Ultra-low profile Pin Socket (for MCU board) 
- Round machine pin x 12 (for MCU board) 
- Mil Max 0305 x 120 (for key switches) 

**And, of course:**

- MCU boards of your choice (Pro Micro, Elite-C, Nice!nano)
- Switches and keycaps.

**Useful quality-of-life tools (links are only for a reference):**

- Masking tape like [this one](https://www.amazon.com/AmazonBasics-Masking-Tape-Inch-Rolls/dp/B07QHSKGMH)

- M2 hex nut driver like [this one](https://www.amazon.com/uxcell-Non-Magnetic-Point-Driver-3-Inch/dp/B07DXZJQ4S/ref=sr_1_40?dchild=1&keywords=Hex+Nut+Driver+m2&qid=1619655993&s=hi&sr=1-40)
- M2 hex driver like [this one](https://www.amazon.com/gp/product/B001ATKWJY/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1) 
- or, all-in-one driver set [this one](https://www.amazon.com/iFixit-IF145-299-4-Driver-Bit-64pc/dp/B0189YWOIO/ref=sr_1_5?dchild=1&keywords=driver+kit&qid=1620838333&sr=8-5)

## Assembly Order

1. Soldering on PCB: MCU Board sockets and right angle headers
2. Switch Plate Assembly
3. (if your build is soldered) Keyboard Switches
4. (if your build is hot-swappable) Hot-swap sockets
5. MCU board onto the PCB
6.  (if your build is wireless) Battery and external Switches

## Assembly instruction

### Step 1. Soldering on PCB: MCU Board sockets and right angle headers

On the Group buy version, all the essential parts are pre-soldered. Make sure if there are any missing components on the PCB:

- Diodes
- Capacitors
- Two on-board slide switches
- Reset switch
- RGB Underglow LEDs
- Resistor (optional part for a buzzer)

![pcb](Vanana-BuildGuide-rev2.5.assets/pcb.jpeg)

For non-GB versions, solder the electronic parts referring to the photo above.

All you have to solder on the PCB are MCU board sockets and right angle headers. 

**Parts you need:**

- Ultra-low MCU board sockets **or** straight pin headers. 
- (wireless setup only) 3 x 2 pos Right angle headers.
- (only when enabling RGB underglow or using a rotary encoder at the position 2 with Elite-C or Nice!nano)  1 x 3 pos Right angle header.
- (non-GB version only) 2 x onboard SMT switches.

**Note**: On the GB version PCB, onboard SMT switches are pre-soldered.

![prep-03](Vanana-BuildGuide-rev2.5.assets/prep-03.jpg)

**Steps**:

1. You can use ultra-low profile sockets (for a hot-swap build) **or** straight pin headers (for a soldered build). The photo below shows compatible sockets and headers. You will use **one of them** depending on your build. 
2. Make sure the height of the insulation (black plastic part in the photo below) is less than or equal to 3mm. Most straight pin headers that come with MCU board has a 3mm insulation. 
3. Insert sockets or headers from the back of the PCB. Masking tape will help you secure the parts when soldering the parts.
4. Solder the pins of sockets or headers from the front of the PCB.
   ![IMG_1690](Vanana-BuildGuide-rev2.5.assets/IMG_1690.JPEG)
   ![IMG_1697](Vanana-BuildGuide-rev2.5.assets/IMG_1697.JPEG)

5. Note that there are two on-board switches on both sides of the PCB. One is for RGB and the other is for Power switch. (Down: OFF/ Up: ON). If you are building a **wired Vanana**, just toggle up the switches and skip to the next section (2. Switch Plate Assembly). If you are building a **wireless Vanana with a plate case kit**, you will use these two on-board switches instead of external switches, so you can also skip to the next section.
   ![IMG_1699](Vanana-BuildGuide-rev2.5.assets/IMG_1699.JPEG)
   ![IMG_1698](Vanana-BuildGuide-rev2.5.assets/IMG_1698.JPEG)

6. If you are building a **wireless Vanana with 3D printed cases**, it is time to solder 3 x right-angle pin headers to use external switches and battery. 
   - NOTE: At the time of designing the board, the RGB switch was added to cut off the quiescent current draw of LEDs. Now the software underglow control of ZMK is equivalent to the hardware switch, so you can skip soldering the RGB switch header, if you do not want to use a hardware switch to control RGB underglow.
7. Place the right-angle pin headers on the back of the PCB as show in the photo below. You may want to use a tape to secure the headers.
   ![IMG_1702](Vanana-BuildGuide-rev2.5.assets/IMG_1702.JPEG)
8. Solder the pin headers from the front of the PCB. For a clean look, you can solder the header with a little soldering iron first, clip off excessive pins, and then reflow soldering by adding more soldering iron. ''
   ![IMG_1704](Vanana-BuildGuide-rev2.5.assets/IMG_1704.JPEG)

9. Done!

### Step 2. Switch Plate Assembly

**Parts you need:**

- 10 x m2 screws 
- 10 x short m2 standoffs

**Steps**:

1. You are free to change the positions of screws at your preference. The ones marked red in the photo above are the recommended locations.
   ![IMG_1674](Vanana-BuildGuide-rev2.5.assets/IMG_1674.JPEG)

2. Insert screws into the switch plate from the top.

3. Insert **short M2 standoffs** (4mm one in GB version kits) and tighten them (I usually do this with hands. However, if you want a rock-solid build, use a small plier and m2 hex screw driver to tighten them). 
   ![prep-02](Vanana-BuildGuide-rev2.5.assets/prep-02.jpg)
   ![IMG_1679](Vanana-BuildGuide-rev2.5.assets/IMG_1679-1621565266916.JPEG)

   ![IMG_1677](Vanana-BuildGuide-rev2.5.assets/IMG_1677.JPEG)

4. If you like to use rotary encoders, which are optional, solder a rotary encoder on the PCB **BEFORE** assembling the PCB and the switch plate.

   - Vanana GB version supports rotary encoders at two positions. A rotary encoder at the position 1 is supported by all Pro Micro compatibles and Nice!nano by default. However, only Nice!nano and Elite-C supports a rotary encoder at the position 2 because it uses extra GPIO pins on Elite-C and Nano, which will be covered in the later section. Likewise, RGB underglow is supported only with Elite-C and Nice!Nano.

5. Assemble the PCB and the switch plate. Place **the long standoffs** (5mm one in the GB kits) and tighten them. Note that the assembled PCB and the switch plate in the photo below does not have a rotary encoder, which may not be your case. 
   ![IMG_1709](Vanana-BuildGuide-rev2.5.assets/IMG_1709-1621572261979.JPEG)
   ![IMG_1710](Vanana-BuildGuide-rev2.5.assets/IMG_1710.JPEG)

### Step 3. (if your build is soldered) Keyboard Switches

**Parts you need:**

- 60 x keyboard switches

1. Vanana GB version supports three layouts. Choose your layout and insert switches into the appropriate positions.

   - Layout C was added by a request of a user who had brachydactyly, and it was to move the spacebars closer to thumb positions.  It is small difference, but I hope it will help at least to some degree.

2. Solder the key switches from the back of the PCB.  

   ![switches_placed.jpg](Vanana-BuildGuide-rev2.5.assets/prep-04.jpg)
   ![IMG_1712](Vanana-BuildGuide-rev2.5.assets/IMG_1712.JPEG)
   ![switches_placed](Vanana-BuildGuide-rev2.5.assets/switches_placed.jpg)
   <u>(Image courtesy: [Aberardinelli](https://github.com/aberardinelli/vananabuild))</u>
   ![switches_soldered.jpg](Vanana-BuildGuide-rev2.5.assets/switches_soldered.jpg)
   (Image courtesy: [Aberardinelli](https://github.com/aberardinelli/vananabuild))

### Step 3. (if your build is hot-swappable) Hot-swap sockets

**Parts you need:**

- 120 x 0305 Mill-Max hotswap sockets (or 7305)

**Steps:**

1. If your build is hot-swappable, you will use 0305 or 7305 hotswap sockets.

2. Place hotswap sockets into the switch holes on the PCB. A precision tweezer will be your life saver. 

   - My favorite way of installing 0305 sockets is to solder them on one or two columns at a time with a masking tape. Place the sockets onto the columns, secure them with a masking tape from the front of the PCB, then solder them from the back of the PCB. Repeat until you get all the sockets soldered.
   - If this is the first time, I highly recommend to practice with at least a few sockets on a scrap board. I would not say it is hard, but it does require a slow progress and some degree of patience. Check some video [tutorials](https://www.youtube.com/watch?v=wmkTVsZ97Vk).
   - Do not put an excessive amount of soldering iron. Use the amount of solder iron that is just enough to fill the gaps between the socket and the hole. 

   ![IMG_1720](Vanana-BuildGuide-rev2.5.assets/IMG_1720.JPEG)

   ![IMG_1716](Vanana-BuildGuide-rev2.5.assets/IMG_1716.JPEG)
   ![IMG_1718](Vanana-BuildGuide-rev2.5.assets/IMG_1718.JPEG)
   ![IMG_1723](Vanana-BuildGuide-rev2.5.assets/IMG_1723.JPEG)

### Step 4. MCU board Assembly.

**Parts you need:**

- MCU board: Pro Micro compatibles or Nice!nano

**Steps:**

1. (optional) If you use Elite-C or Nice!nano to enable RGB underglow or use the rotary encoder at the encoder position 2, the following mod will be useful. This mod was to make the connections easier with Dupont cables, but you can also skip this part and solder the wires to make a soldered connection between the extra GPIO pinouts of MCU boards and the PCB. 

   - My preferred way of doing this is to place a right angle header, cut the excessive header pins, secure the header pins with a masking tape, and solder it on the board. 

   ![IMG_1708](Vanana-BuildGuide-rev2.5.assets/IMG_1708-1621577063751.JPEG)
   ![IMG_1707](Vanana-BuildGuide-rev2.5.assets/IMG_1707-1621577298729.JPEG)

2. The rest is straightforward. If you used a regular straight pin headers on the PCB, place the MCU board on it and solder them. If you are used ultra-low profile hotswap sockets, place the MCU board on it, insert compatible machine pins, and apply soldering. 
   ![IMG_1725](Vanana-BuildGuide-rev2.5.assets/IMG_1725-1621577576533.JPEG)

3. Now, Connect the extra GPIO pins of the MCU board to PCB using the **short** Dupont cables included. 
   ![prep-06](Vanana-BuildGuide-rev2.5.assets/prep-06.jpg)
   ![prep-07](Vanana-BuildGuide-rev2.5.assets/prep-07.jpg)

### Step5. (wireless build only) External switch and battery assembly

If you are building a wired build, you can skip this section. I personally found that this step is the most difficult part because... I have fat fingers.

**Parts you need:**

- 2 x Long Dupont cable (for an external power switch connection)
- 2 x Long Dupont cable (for an external power switch connection)
- 3 x Short Dupont cable (for a MCU board connection)
- 2 x Short Dupont cable (for a battery connection)
- 4 x Short m2 screws
- 4 x m2 nuts

**Steps:**

1. The process is quite simple. Place the external switches and assemble them with short m2 screws and nuts included. 
   - The best strategy that I found was that I found was to hold the nuts with a precision tweezer and tighten the screws using a m2 hex screw driver.
     ![IMG_1737](Vanana-BuildGuide-rev2.5.assets/IMG_1737.JPEG)
2. Connect the the switches to the PCB using the long Dupont cable.
   - Note that the on/off directions of the switches depend on the cable arrangement in this step.
3. Prepare the battery of your choice. 
   - The Vanana cases have a recessed area to place a battery. The maximum size of a battery for the GB version is 45mm(W) x 55mm(D) x 5mm(H). 
4. Solder two Dupont cables to a battery of your choice. This will make it easy to replace the batteries. 
5. Connect the battery to the PCB using the long Dupont cable. 
   - **IMPORTANT**!!: The battery pinout on the board has polarity. MAKE SURE TO CONNECT WIRES OF A BATTERY TO THE RIGHT PINOUT. In most cases, the red wire of a battery is +, and the black is -. However, double check the polarity of your battery.
   - In order to secure the battery onto the case, you may want to use a thin double sided tape. Also, if you are using 0305 hotswap sockets, the tip of the sockets may touch your battery when you close the case. Consider to apply a thin non-conductive electrical tape to prevent them poke into the battery.



### Step 6. Closing the case.

**Parts you need:**

- 10 x m2 nuts
- 10 x m2 washers

**Steps:**

1. We are there. close your case with the PCB assembly using m2 nuts and washers.
   - Washers are optional. However, it will help reduce the possible damage to he case, which could be caused by over-tightening nuts or prolonged time of use.  



# Vanana (rev 2.5 GB) Firmware guide

At the time of writing, the QMK Vanana firmware has been merged to the official repository, and the ZMK firmware has been uploaded to the support GITHUB account. My knowledge about these firmware is limited and is just enough to write new firmware for a new keyboard. If you encounter problems in using these firmware packages, the best resources to solve your issues are the official documentations and Discord servers. Here I briefly describe the easiest way of making your own firmware using QMK and ZMK. Please note that these pipelines are created by awesome QMK and ZMK communities, we do not deserve any credits for these processes. 

## QMK firmware (wired only)

The best way to start using QMK firmware is to check the official [documentation](https://docs.qmk.fm/#/) and Discord server.

1. Head over to QMK Configurator, and look for Vanan rev 2. 
2. Configure your keymaps
3. Save your keymap as a json file for later use/modifications.
4. Compile your kemaps
5. When the compilation has been finished, download a hex file.
6. Install QMK toolbox. 
7. Run QMK toolbox, load the downloaded firmware using the Open button.
8. Connect your Vanana to computer, click the reset button of Vanana twice, which are placed on the back of the keyboard.
9. Click Flash on QMK toolbox. 
10. Enjoy Vanana with QMK

ZMK firmware

1. Register to GITHUB
2. Fork dELIKEEb zmk-config repository into your account
3. change the keymap, and press the commit button. 
4. each time when you hit the commit button, A firmware compilation will be performed on cloud. You can find the compiled firmware at workflwo.
5. Download the firmware and unzip it. 
6. You will see a Vanana firmware file among the unzipped files. 
7. Connect your Vanana to computer, click the reset button of Vanana twice, which are placed on the back of the keyboard.
8. Vanana will appear as an external drive. 
9. Copy and paste the firmware to the Vanana drive. 
10. Enjoy Vanana with ZMK

Note on ZMK firmware:

1. Take a look at Vanana's default keymap with [ZMK keycodes]() to see the default key allocation. 
2. By default, 1 to 5 keys on Layer 3 (Lower + Raise keys) are allocated to the BT profiles. 
3. ESC on Layer 3 turns VANANA into the bootloader mode.
4. Backspace  on Layer 3 deletes the BT connection of the current profile. 
