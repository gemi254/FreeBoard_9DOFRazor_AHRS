FreeBoard_9DOFRazor_AHRS
========================
Freeboard 9 Degrees of freedom Measurement Heading Reference System with 9DOF Razor IMU 
This code transforms a Razor IMU to a NMEA Measurement Heading Reference System to use 
it with navigation software like freeboard and opencpn.

Compile this file using arduino IDE and upload the binarry file to a
9 Degrees of Freedom - Razor IMU - https://www.sparkfun.com/products/10736
in order to use it as Heading reference system with NMEA sentences

Upload the project with an FDTI adapter and connect to the serial port
with speed 38400 

send..
"#FBF" -> to return to razor mode 
"#on"  -> to begin calibration

send
"ALG=90" to align the sensor to 90 degress to the installation
"DEC=0.2" to set the magnetic variation

Follow the steps needed to complete the calibration to the razor  IMI
and copy the calibration data to the source.
uncomment 
"#define CALIBRATION__MAGN_USE_EXTENDED true"
and  re-compile the file with the calibration data.

Upload the hex file and connect Razor IMU with the freeboard via USB port..

