# CMPE242
Work

Steps to Build the device driver and executable files
1) As this project deals with manipulation of character device drivers, go to the character device driver folder under /opt.

2) Add the device driver file present in GitHub to the char folder.

3) Edit the Kconfig file to accommodate the new device driver.

4) Edit the menuconfig file to accommodate the new device driver

5) Navigate to linux-2.6.38 folder under opt and type in make menuconfig
      
6) In the Kernel configuration window, navigate to Device Drivers -> Character Devices -> 'The driver that you created'

7) Configure it to build as a module

8) In the command prompt, type in 'make device_driver_filename.ko'

9) Navigate to the application's folder (examples folder) and add the application file which is present in GitHub there.

10) Build the application file by typing in 'make app_filename'

Steps to Transfer the files to the ARM board
1) Transfer the device_driver.ko file and the executable file form the char and examples folder respectively to the USB Flash drive

2) Plug in the USB Flash drive to the USB port1 in the ARM board

3) You might require Putty to transfer the file. If you dont have it, download it by typing the following in the terminal
    sudo apt-get install s

4) Typ
