
## Read Only Memory (ROM)
- located on the motherboard
- contain instructions accessed by CPU
- includes booting and loading the OS
- non volatile
##### ROM Chip
- written when manufactured
- cannot be erased or written - is obsolete now

##### PROM
- programmable read only memory
- manufactured blank, then written to when needed
- write once and cannot be erased

##### EPROM
- erasable programmable read only memory
- non volatile
- can be erased via strong UV light
- transparent quartz window
- constant changing can render chip useless

##### EEPROM
- electrically erasable programmable read only memory
- AKA "flash ROMs"
- often used to store BIOS and microcontrollers

## Flash Memory
##### NOR Flash
- non volatile memory
- used to store firmware like BIOS/UEFI
- fast random access
- high reliability
- suitability for critical system processes
- often used in embedded systems 

##### NAND Flash
- most popular in the market
- NAND gate is opposite of AND gate
- commonly used for mass storage in SSDs, USB flash drives, and in computers for firmware

##### SPI Flash
- serial interface
- used for storing networking, consumer, automotive, medical, gaming, communication, and IoT devices

## Memory
##### Buffered Memory (RDIMM)
- includes buffer between IMC and DRAM chips
- register between IMC and actual memory
- helps to control electrical load on memory bus
- when you add more memory the electrical load on the bus increases
- improves system load and integrity

##### Memory CAS Latency
- Column Address strobe latency (CAS)
- CAS latency is measured in clock cycles
- lower CAS latency gives better memory performance

##### Error Correcting Code (EEC)
- includes additional bits for error detection and correction
- improves reliability

##### Timing Parameters
- memory module performace
- measures clock cycles
- four parameters (ex. 5-5-5-15)
	- cas latency
	- tRCD row to column address
	- tRP row precharge time
	- tRAS row active time
#### Serial Presence Detect (SPD)
- stored on EEPROM chip
- located on SDRAM
	- module size
	- data width
	- speed
	- voltage
## Expansion Cards
- aka dedicated cards
- designed to use particular expansion bus standard
- supports plug and play
- supports **full duplex** - **simultaneous bidirectional data transfer**

##### PCIe (peripheral component interconnect express)
- defines x2, x4, x8, x16, and x32
	- x1 is one lane transmission
	- x16 is sixteen lane transmission
	- GPUs are x16
- cross size compatible
	- smaller cards can fit in larger PCIe slots
	- x4 card can fit in 8x slot
- Safeslot
	- orginally by ASUS
	- for x16
	- reinforced slot with metal frame that provides additional structural support
- multiple Gbps by 8 to get GBps
![[Pasted image 20231005110733.png]]
![[Advanced Components-1697917740289.jpeg]]