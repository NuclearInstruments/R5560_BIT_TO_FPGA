# R5560 FPGA file generator
This Python scripts convert an input BIN file, generated by vivado in a FPGA file that can be stored the /mnt/sdcard/firmware.fpga to automatically load it at linux startup

Usage:

	python bintofpga.py binaryfile.bin firmware.fpga

then copy the file via scp

	scp firmware.fpga root@r5560_ip_address:/mnt/sdcard/firmware.fpga

Log to R5560 via SSH or serial, enter 

	sync
	reboot

