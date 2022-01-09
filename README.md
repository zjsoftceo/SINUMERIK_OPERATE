# Grbl-1.1z
*********************************************************************
- Date: 2022-01-08
- Author: Zhang Jiang 
- Subject: Arduino_Grbl_CNC Grbl v1.1z.20220108
- Copyright (c) 2022 Zhang Jiang For The Sunflower Tech LTD,China
------------------------------------------------------------------------------------
An open source, embedded, high performance g-code-parser and CNC milling controller
written in optimized C that will run on a straight Arduino UNO

To use:
- First make sure you have imported Grbl source code into your Arduino
  IDE. There are details on our Github website on how to do this.

- Select your Arduino Board and Serial Port in the Tools drop-down menu.
  NOTE: Grbl only officially supports 328p-based Arduinos, like the Uno.
  Using other boards will likely not work!
 
TO Updata G-Code:
- #define MODAL_GROUP_G5 5 // [G93,G94,G95] Feed rate mode
- Modal Group G5: Feed rate mode
- #define FEED_RATE_MODE_UNITS_PER_REV  2 // G95 (Zhang Jiang)
- case 95:
- word_bit = MODAL_GROUP_G5;
- gc_block.modal.feed_rate = 95 - int_value;
- break;

*********************************************************************
