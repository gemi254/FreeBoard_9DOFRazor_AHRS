FreeBoard_9DOFRazor_AHRS
========================

Freeboard 9 Degree of Measurement Heading Reference System with 9DOF Razor IMU

Compile this file and upload the binarry file to a
9 Degrees of Freedom - Razor IMU - https://www.sparkfun.com/products/10736
in order to use it as Heading reference system with NMEA sentences

Upload the project with an FDTI adapter and connect to the serial port
with speed 38400 

send..
"#FBF" -> to return to razor mode 
"#on"  -> to begin calibration

Follow the steps needed to complete the calibtration and at the end
use 
"#define CALIBRATION__MAGN_USE_EXTENDED true"
and  re-compile the file with the calibration data.
Upload the hex file and connect Razor IMU with the freeboard..

