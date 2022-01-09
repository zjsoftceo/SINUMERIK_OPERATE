****
    Not supported:
  - Canned cycles
  - Tool radius compensation
  - A,B,C-axes
  - Evaluation of expressions
  - Variables
  - Override control (TBD)
  - Tool changes
  - Switches
****  
 -  (*) Indicates optional parameter, enabled through config.h and re-compile
    - group 0 = {G92.2, G92.3} (Non modal: Cancel and re-enable G92 offsets)
    - group 1 = {G81 - G89} (Motion modes: Canned cycles)
    - group 4 = {M1} (Optional stop, ignored)
    - group 6 = {M6} (Tool change)
    - group 7 = {G41, G42} cutter radius compensation (G40 is supported)
    - group 8 = {G43} tool length offset (G43.1/G49 are supported)
    - group 8 = {M7*} enable mist coolant (* Compile-option)
    - group 9 = {M48, M49, M56*} enable/disable override switches (* Compile-option)
    - group 10 = {G98, G99} return mode canned cycles
    - group 13 = {G61.1, G64} path control mode (G61 is supported)
****
Supported G-Codes in v1.1z 20220108
****
 - G0, G1: Linear Motions
 - G2, G3: Arc and Helical Motions
 - G4: Dwell
 - G10 L2, G10 L20: Set Work Coordinate Offsets
 - G17, G18, G19: Plane Selection
 - G20, G21: Units
 - G28, G30: Go to Pre-Defined Position
 - G28.1, G30.1: Set Pre-Defined Position
 - G38.2: Probing
 - G38.3, G38.4, G38.5: Probing
 - G40: Cutter Radius Compensation Modes OFF (Only)
 - G43.1, G49: Dynamic Tool Length Offsets
 - G53: Move in Absolute Coordinates
 - G54, G55, G56, G57, G58, G59: Work Coordinate Systems
 - G61: Path Control Modes
 - G80: Motion Mode Cancel
 - G90, G91: Distance Modes
 - G91.1: Arc IJK Distance Modes
 - G92: Coordinate Offset
 - G92.1: Clear Coordinate System Offsets
 - G93, G94,G95: Feedrate Modes (G95 Gode: Zhang Jiang)
 - M0, M2, M30: Program Pause and End
 - M3, M4, M5: Spindle Control
 - M7 , M8, M9: Coolant Control
 - M56: Parking Motion Override Control
 - (*) denotes commands not enabled in config.h by default.
****
