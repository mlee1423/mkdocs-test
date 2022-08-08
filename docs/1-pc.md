# Beginner's Introduction Guide for PC Building
## Introduction


### Components
Inside the case of every computer is the following:

* CPU
* CPU Cooler
* Motherboard
* Memory
* Graphics Card
* Storage
* PSU

#### CPU - Central Processing Unit
The CPU's job is to execute instructions for software running on the computer. It is recommended the builder know the number of cores and thread count of each CPU being considered for purchase and installation. All CPUs have cores, but recent CPUs split each core into two virtual cores called threads, adding up to 30% extra performance. The more CPU cores, the more applications can be run on the machine at the same time without issue.

#### Socket Types and Compatible Motherboards

|Processor | Socket | Compatible Motherboard |
|:-------:|:-------:|:-------:|
|Core i9/i7/i5/i3-12XXX | LGA1700 | Z690 Platform |
|Core i9/i7/i5/i3-10XXX | LGA1200 | Z490/Z590 Platform |
|Core i7/i5/i3/Pentium/Celeron | LGA 1151 | Z390 Platform |
|Core X-Series Processor | LGA 2066 | X299 Platform |
|AMD Ryzen | AM4 | B450/A320/X470/B550/X570 Platform |
|AMD Ryzen Threadripper | sTRX4 | TRX 40 Platform |

#### CPU Cooler
CPUs produce a lot of heat. High temperatures can cause the system to shut down in order to protect important components, and may even cause permanent damage. Fans and heatsinks are therefore necessary in order to keep the CPU running cool. With the exception of some high-end CPUs, most boxed CPUs are bundled with a corresponding CPU cooler which can meet basic demands for heat dissipation. For better system performance, it is suggested to buy a better CPU cooler.

Coolers can be classified in terms of heat dissipation medium into two types: liquid cooling and air cooling. Air coolers can be further classified into tower-style, downdraft, and updraft coolers, depending on their appearance and airflow direction. Builders should choose a cooler that fits the case and circumstance.

##### Consider the Following
* Coolers need to provide corresponding brackets, as bracket positioning may vary slightly depending on the socket on the motherboard.

* Each CPU cooler supports a different thermal design power (TDP), indicating the upper range of heat output that it can handle. More powerful CPUs need better coolers to ensure stable operation.

* Choose a cooler that fits the PC Case. Powerful coolers often have large heat sinks, so it is important to choose a cooler that can fit into the case without obstructing other components.

#### Motherboard
The motherboard, also called the mainboard, links all the components of the computer, connecting the processor, memory modules, graphics and expansion cards, hard drives, and connections to the network, keyboard, mouse, and more.

##### Dimensions
Common motherboard sizes include:

* ATX (30.5cm x 24.4cm)
* Micro-ATX (24.4cm x 24.4cm)
* Mini-ATX (17cm x 17cm)

##### Chipsets
For a given CPU, there's often a choice of chipsets that support it. The chipset provides options and connectivity on the motherboard, and higher priced chipsets offer more features. The higher the chipset number, the more functionality the motherboard will have. Below is a table of Intel and AMD's most common compatible chipsets.

| 12th Gen Intel Core | AMD Ryzen|
|:------:|:------:|
|H160|B550|
|H670|B450|
|B660|X570|
|Z690|X470|

##### Overclocking
In order to overclock a processor, the overclocker intentionally increases the CPU operation frequency above the original stock specifications. Because the processor's frequency heavily impacts the effective computational speed of the CPU, the ultimate goal is to increase the frequency of the CPU in order to achieve faster performance.

!!! warning
    If a motherboard that supports overclocking is purchased, it may require dual ATX 8 pin or 8+4 pin for the CPU. Check to make sure the selected power supply has them.

#### Memory - RAM
Random Access Memory (RAM) is used to load and run applications, respond to commands, or toggle between multiple programs. Memory is almost always being actively used by the PC operating system. Below is a table showcasing what types of tasks can be done with different amounts of RAM.

| 4GB | 8GB | 16GB | 32GB | 64GB+ |
|-----|-----|------|------|------|
|Typically installed on low-end Chromebooks and select tablets, only to consider on extreme budget constraint | Usually installed on entry-level notebooks. Fine for basic Windows tasks and games at low settings, but runs out of steam quickly| Excellent for systems doing multiple tasks and gaming at normal settings | Installed on most professional workstations and good for gaming on ultra settings | For purpose-built workstations only |

Different programs require different amounts of RAM, but regardless of the application, it's likely to use a small amount. Adding up over time, if too much RAM is being used at one time, the applications currently being used will slow down severely.

#### GPU - Graphical Processing Unit
A GPU, or graphics card, is an expansion card that fits into the PCIe slot on the motherboard. It handles complex graphical instructions, computing images, textures and objects, and sends the result to one or more monitors. The motherboard may have HDMI, DisplayPort, or older DVI or VGA ports, driven by the integrated graphics GPU inside some processors.

#### Storage
Storage has evolved from hard drives that use magnetic technology to store data on spinning disks. Reaching 20 terabytes (TB) or more, 4 to 8 TB drives are a cost-effective option for mass storage. But, with data transfer around 140 or 180 megabytes (MB) per second, speed is far surpassed by Solid State Drives (SSDs) and SATA m.2 drives.

#### PSU - Power Supply
Power supply is important when building a PC, as it converts AC power into DC power for the CPU, motherboard, graphics card, and all peripherals. General guidelines are as follows: 500-600 Watts for a PC using the web and office apps, 650-850 Watts for a PC using any external GPU. Check the selected GPU's power requirements for exact measurements.

##### Energy Efficiency
The 80 Plus certification program for power supply units offers 80 Plus, 80 Plus Bronze, 80 Plus Silver, 80 Plus Gold, 80 Plus Platinum and 80 Plus Titanium certification levels. The most efficient (and most expensive) Titanium tier offers more than 90% energy efficiency.

The 80 plus bronze, silver, gold, platinum and titanium ratings have 2 to 3 percent efficiency gains between tiers, starting with bronze at 82 percent, and titanium having 92% efficiency, though that comes with a price. Modular power supplies can reduce cable clutter in the PC case, and can make wiring components and cable management easier. And note that CPU and PCI 6+2 connectors may look the same, but they won't fit each other's sockets.

##### Power Supply Design
Below is a table covering the different pros and cons between the three PSU types on the market.

| | Full Modular| Semi Modular | Non Modular|
|----|----|----|----|
|Air Flow | Excellent air flow due to less cable clutter | Good air flow with good cable management | Bad air flow due to cable clutter |
| Temperature | Low temperature reading due to less cable clutter | Fine temperature reading due to good air flow and cable management | Poor cable management will result in high temperature |
|Aesthetics | Easy to organize and manage for good looks | Good looks with decent cable management | Messy looks due to too many cables|
|Convenience | Convenient PSU replacement | Easier PSU replacement with less cables to unplug | Need to remove all cables when switching PSU |
|Customization | Can be fully customized | Limited customization options | No customization options |

#### Case
Selecting a case can be done mostly to personal taste, but there are a few factors to keep in mind. First, the case needs to have good air flow, so there should be lots of fan mounting spots. Also look for wide openings at the front for air to enter, and having them filtered will help keep dust out of the case. Second, check what size motherboard the case will accept, most motherboards are ATX sized and won't fit in smaller cases. Third, check the length of GPU the case accepts, as newer graphics cards can reach 27-33cm in length. Fourth, check the case for mounting spots for all storage devices.

For air cooling, check the case's maximum CPU cooling height in millimeters, having at least a few mm more than the height of the actual cooler. For liquid cooling, the radiator needs a spot to mount to the case, so check for 240 or 360mm rad mounting locations at the front or the top. The top is the recommended location for keeping the inside of the case cool as the rad will exhaust directly outside the case. Never mount the rad at the bottom of the case, the pump should never be at the very top of a liquid loop as the small amount of air in the loop will want to pool there, reducing the efficiency of the CPU coldplate and pump.

Finally, case construction. Tempered glass panels show off the internals but add considerable weight, and care must be taken when transporting and after installation, being careful not to torque fasteners too tightly on the glass as over time this can cause it to shatter.

### Operating Systems
An operating system is considered to be the backbone of any system. Without an operating system, the user and system cannot interact. The three most universally used operating systems are Windows, MacOS, and Linux. Windows is developed by Microsoft and is comparatively the most accessible operating system on the market. MacOS is developed by Apple for their Macintosh systems and is geared towards users that want performance fused with simplicity. Lastly, Linux is an free, open-source family of operating systems initially developed by Linus Torvalds and later added onto by the GNU Project and the Linux community. It is mainly used by enthusiasts and companies that run servers and applications with the need of high security and no downtime. Below is a table comparing the systems.

| Windows | MacOS | Linux |
|:-------:|:-----:|:-----:|
| easy access | easy user experience | easy on the wallet |

#### Dual Booting


#### Virtual Machines
Virtualization is the process of creating a software-based, or "virtual" version of a computer, with dedicated amounts of CPU, memory, and storage that are "borrowed" from a physical host computer—such as your personal computer— and/or a remote server—such as a server in a cloud provider's datacenter. A virtual machine is a computer file, typically called an image, that behaves like an actual computer. It can run in a window as a separate computing environment, often to run a different operating system—or even to function as the user's entire computer experience—as is common on many people's work computers. The virtual machine is partitioned from the rest of the system, meaning that the software inside a VM can't interfere with the host computer's primary operating system.
