# nvme_controller_emulator
![build_status](https://travis-ci.org/himaaaatti/nvme_controller_emulator.svg?branch=master)

## build
```
$ gmake build
```

## Tasks

- initialization  
Initialization steps are defined at Section 7.6.1 in NVMe specification. Controller emulator must has below functions.  

	- [x] PCI configuraion registers
	- [x] MSI/MSI-X registers
	- [x] NVMe controller register 
		- [x] AQA (admin queue attirubte)
		- [x] ASQ (admin submission queue)
		- [x] ACQ (admin completion queue)
	- [x] doorbell registers
		- [x] Admin sumbmission queue doorbell register
		- [x] Admin completion queue doorbell register

	- [x] Admin Commands
		- [x] Set Feature
			- [x] Number of Queues
			- [x] Asynchronous Event Configuration
            - [x] Interrupt Coalecing
        - [x] Get Feature
            - [x] Temparture Threshold

		- [x] Create I/O Completeion Queue
		- [x] Create I/O Submission Queue
        - [x] Identify
            - [x] Identify Controller data structure

- read and write data via this nvme controller emulator
	- [ ] Read
		WIP
	- [ ] Flush
	
//TODO list up
