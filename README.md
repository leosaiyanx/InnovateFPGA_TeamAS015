# InnovateFPGA_TeamAS015
Flex Force Smart Glove InnovateFPGA Contest

Smart Glove project created for the InnovateFPGA contest

Introduction:

According to the 2013 update report of the American Heart Association (AHA) [1], each year approximately 795,000 people suffer from stroke, which makes it the leading cause of permanent disability in the country. Recent advances in development of robotic devices have demonstrated the feasibility and increased benefits of robotic-assisted rehabilitation for stroke-related or joint injuries of the upper extremities [2]-[4]. Research shows that the human brain is capable of self-reorganizing (i.e. plasticity), especially after limb stimulation is employed, resulting in re-establishment of neural pathways that control volitional movement. Traditional physical therapy, which involves one-on-one interaction with a therapist is a conventional method used for stimulating sensorimotor activities, while robotic-assisted rehabilitation can increase the effectiveness of the repetitive exercises used in rehabilitation. Furthermore, to properly quantify the effectiveness of both conventional and robotic-assisted upper-limb rehabilitation, sensorimotor measurements need to be acquired and analyzed. Thus, the invention of the Flex Force Smart Glove (FFSG) allows for a complete nonintrusive design used to acquire and analyze sensorimotor information obtained from the human hand.

A nonintrusive and noninvasive Flex Force Smart Glove (FFSG) design is presented that allows for acquisition and processing of sensorimotor information obtained from the human hand. The novel FFSG design is powered by the Intel Altera FPGA and incorporates all the sensors needed to measure the force and rotation of the human wrist and fingers. Quaternion-based Kalman filters are used to fuse the raw sensor data from five finger joints and one wrist joint to provide detailed orientation information. In addition, feed forward neural network filters are used to classify possible hand exercises that can be further used to facilitate rehabilitation through exercise sessions. The novel design will allow for a unified way to quantify the effectiveness of both conventional and robotic-assisted rehabilitation.

For more details visit the InnovateFPGA page:
http://www.innovatefpga.com/cgi-bin/innovate/teams.pl?Id=AS015

YouTube Video Demonstration can be found here:
https://www.youtube.com/watch?v=oGvOwnDhRaQ


Programming FPGA
Hardware Requirements:
- FPGA Programming Mode: Passive Parralel x 16 (Jumpers set to all ON)

1. Program Pre-loader

  --> Run the following command as "Admin"
  --> alt-boot-disk-util.exe -p preloader-mkpimage.bin -a write -d g
  

2. Copy the remaining files in the sd_card_boot_files directory to the FAT file system on the SD card

Software

1. Build the main project in the HPS_FPGA_FFSG directory 

2. Copy the executable HPS_FPGA_FFSG to the DE10-nano via FTP 

3. Make the HPS_FPGA_FFSG program executable on the DE10-nano by runnig "chmod +x HPS_FPGA_FFSG" in the directory that the file was placed

4. Run the executable, it will ask for PWM value (for testing), enter any integer value to observe the LED dim according to the PWM rate and begin using the FFSG menu to test all of the sensors or stream to a local host



References
1. Heart disease and stroke statistics - 2013 Update American Heart Association

2. N. Hogan, H.I. Krebs, J. Charnnarong, P. Srikrishna and A. Sharon, "MIT-MANUS: A Worskstation for manual therapy," Proc. of IEEE International Workshop on Robot and Human Communication, pp. 161-165, 1992

3. H.I. Krebs, N. Hogan, M.L. Aisen and B.T. Volpe, "Robot-aided neurorehabilitation," IEEE Trans on Rehabilitation Engineering, Vol. 6, No. 1, pp. 75-87, 1998

4. Z.Bien, M.J. Chung, P.H. Chang, D.S. Kwon, D.J. Kim, J.S. Han, and J.H. Kim, “Integration of a Rehabilitation Robotic System (KARES II) with Human-Friendly Man-Machine Interaction Units,” Proc. Of Autonomous Robots, pp. 165-191, 2004
