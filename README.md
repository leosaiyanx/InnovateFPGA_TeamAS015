# InnovateFPGA_TeamAS015
Flex Force Smart Glove InnovateFPGA Contest

Smart Glove project created for the InnovateFPGA contest

Introduction:

A nonintrusive and noninvasive Flex Force Smart Glove (FFSG) design is presented that allows for acquisition and processing of sensorimotor information obtained from the human hand. The novel FFSG design is powered by the Intel Altera FPGA and incorporates all the sensors needed to measure the force and rotation of the human wrist and fingers. Quaternion-based Kalman filters are used to fuse the raw sensor data from five finger joints and one wrist joint to provide detailed orientation information. In addition, feed forward neural network filters are used to classify possible hand exercises that can be further used to facilitate rehabilitation through exercise sessions. The novel design will allow for a unified way to quantify the effectiveness of both conventional and robotic-assisted rehabilitation.

For more details visit the InnovateFPGA page:
http://www.innovatefpga.com/cgi-bin/innovate/teams.pl?Id=AS015

YouTube Video Demonstration can be found here:
https://www.youtube.com/watch?v=oGvOwnDhRaQ


Programming FPGA
Requirements:
- FPGA Programming Mode: Passive Parralel x 16 (Jumpers set to all ON)

1. Program Pre-loader

  --> Run the following command as "Admin"
  --> alt-boot-disk-util.exe -p preloader-mkpimage.bin -a write -d g
  

2. Copy the remaining files in the sd_card boot directory to the FAT file system on the SD card

