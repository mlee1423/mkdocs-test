# Beginner's Introduction Guide to PC Building

## Components
Inside the case of every computer is the following:

* CPU
* CPU Cooler
* Motherboard
* Memory
* Graphics Card
* Storage
* PSU

### CPU - Central Processing Unit

![cpu](./assets/images/cpu.png){: style="width:15em"}

The CPU, or Central Processing Unit, is one of the most important parts of any PC. As the primary hub, it processes instructions that come from programs, the operating system, or other components in the computer. Not too long ago, these functions had to be split across multiple processors to be completed, but manufacturing and design improvements have made it so that the entire CPU can fit onto a single chip.

CPUs work in sequence, which means that every instruction set processed can only be executed in order, one after another. This process happens in three stages: fetch, decode, execute. The CPU takes the instruction (fetches), processes it to be able to read it properly (decodes), and then executes it.

#### Cores
![cpucore](./assets/images/cpu core.png){: style="width:15em"}

Originally, CPUs had a single core. Meaning that the physical CPU had just a single central processing unit on it. To increase performance, manufacturers add additional cores. Multicore processors are made up of two or more CPUs on a single chip. The individual cores can execute multiple instructions in parallel, which greatly increases software performance while multi-tasking.

!!! info
    There are two major CPU manufacturers: **Intel** and **AMD**. Both companies frequently trade places for offering better value in terms of cores and threads, without sacrificing too much in the performance department.

#### Threads

``` mermaid
graph TD
A(Dual Core CPU) --- B(Core 1);
A --- C(Core 2);
B --- D(Thread 1);
B --- E(Thread 2);
C --- F(Thread 3);
C --- G(Thread 4);
```
For even greater performance enhancement, manufacturers Intel and AMD began using "hyper-threading" and "simultaneous multithreading (SMT)", respectively. A thread is a virtual version of a CPU core. A single CPU core can have up to two threads per core. While cores increase the number of tasks available to execute at one time, threads improve overall performance by being able to manage the task processes.



!!! example
    Opening an application on a computer creates a **thread** to handle tasks associated with that particular application. Opening and running more applications creates more threads.

    ``` mermaid
    graph LR
    A(Core 1) --- B(Execution Thread 1: Open Chrome Web Browser Application);
    A --- C(Execution Thread 2: Open Spotify Application);
    B --- D(Task Process 1: Accessing Home Page);
    B --- E(Task Process 2: Typing Web Address);
    B --- F(Task Process 3: Loading Web Page);
    C --- G(Task Process 1:  Searching for Artist);
    C --- H(Task Process 2:  Selecting Album);
    C --- I(Task Process 3:  Playing Song);

    ```

#### Sockets
The CPU Socket is where the CPU is housed when installed onto the motherboard. Socket types are built into the motherboard and cannot be changed. Each pin is wired to communicate with a specific part of the system.

#### Chipsets
For a given CPU, there's often a choice of chipsets that support it. A chipset acts as the motherboard's communications center and traffic controller. It determines component compatibility, expansion options, and overclockability.

Below is a table showing common CPUs, their socket type, and corresponding available chipsets.

|Processor | Socket | Chipsets |
|:-------:|:-------:|:-------:|
|Core i9/i7/i5/i3-12XXX | LGA1700 | Z690 Platform |
|Core i9/i7/i5/i3-10XXX | LGA1200 | Z490/Z590 Platform |
|Core i7/i5/i3/Pentium/Celeron | LGA 1151 | Z390 Platform |
|Core X-Series Processor | LGA 2066 | X299 Platform |
|AMD Ryzen | AM4 | B450/A320/X470/B550/X570 Platform |
|AMD Ryzen Threadripper | sTRX4 | TRX 40 Platform |

!!! tip "Simply Put"
    A **socket** determines if a CPU will physically fit and work on that motherboard while the **chipset** determines features and properties the board has. (e.g. A Z170 is the same socket type as H170, but only the Z board can overclock.)

#### Overclocking
In order to overclock a processor, the user intentionally increases the CPU operation frequency above the original stock specifications. Because the processor's frequency heavily impacts the effective computational speed of the CPU, the ultimate goal is to increase the frequency of the CPU in order to achieve faster performance.

### CPU Cooler
![cpufan](./assets/images/cpu fan.png){: style="width:15em"}

CPUs produce a lot of heat. High temperatures can cause the system to shut down in order to protect important components, and may even cause permanent damage. Fans and heatsinks are therefore necessary in order to keep the CPU running cool.

!!! info
    With the exception of some high-end CPUs, most boxed CPUs are bundled with a corresponding CPU cooler which can meet basic demands for heat dissipation. For better system performance, it is suggested to purchase a separate CPU cooler.

Coolers can be classified in terms of heat dissipation medium into two types: liquid cooling and air cooling. Air coolers can be further classified into tower-style, downdraft, and updraft coolers, depending on their appearance and airflow direction.

#### Consider the Following
* Coolers need to provide corresponding brackets, as bracket positioning may vary slightly depending on the socket on the motherboard.

* Each CPU cooler supports a different thermal design power (TDP), indicating the upper range of heat output that it can handle. More powerful CPUs need better coolers to ensure stable operation.

* Choose a cooler that fits the PC Case. Powerful coolers often have large heat sinks, so it is important to choose a cooler that can fit into the case without obstructing other components.

### Motherboard
![mb](./assets/images/mb.png){: style="width:15em"}

The motherboard, also called the mainboard, is a Printed Circuit Board (PCB) that holds and allows communication between the components of a computer. This includes the processor, memory, graphics card, hard drive, as well as any specialty expansion cards. The motherboard also contains the computer's main I/O ports that connect the attached components to peripherals like the keyboard, mouse, webcams, speakers and more.

!!! info
    The motherboard may have HDMI, DisplayPort, DVI or VGA ports driven by the integrated graphics GPU inside some processors.

#### Dimensions
Common motherboard sizes include:

* ATX (30.5cm x 24.4cm)
* Micro-ATX (24.4cm x 24.4cm)
* Mini-ATX (17cm x 17cm)

### Memory - RAM
![ram](./assets/images/ram.png){: style="width:15em"}

Random Access Memory (RAM) is used to load and run applications, respond to commands, or toggle between multiple programs. The speed and performance of the system directly correlate to the amount of RAM installed on the PC. The more programs being run, the more RAM is needed.

#### Capacity Comparison

| 4GB | 8GB | 16GB | 32GB+ |
|-----|-----|------|------|
|Decent. Adequate only for word processing, e-mail, and web browsing. | Standard. Minimum required for gaming.| Great. Ideal for gaming and most system tasks. | Premium. Any kind of system intensive, workstation-grade tasks; programming, virtual machines, photo and video editing. |

!!! bug "Common Virus Scam"
    It is not possible to **download** more RAM. RAM is a **physical** object. This is a common trick to have a user download a virus and infect the PC.

### GPU - Graphical Processing Unit
![gpu](./assets/images/gpu.png){: style="width:20em"}

A GPU, or graphics card, is an expansion card that fits into the PCI-e slot on the motherboard. It handles complex graphical instructions, computing images, textures and objects, and sends the result to one or more monitors.

!!! tip
    Be sure to connect the monitor display cable to the correct display port. A common mistake PC builders make is connecting the monitor of choice to the motherboard's I/O ports instead of the GPU's I/O ports, leading to unexpectedly poor graphic display performance.

#### Performance Comparison

There are two main companies that make most of the GPUs on the current market: **Nvidia** and **AMD**. Below is a table comparing their products by usage and performance class.

| Usage | Performance | GPU |
|-----|-----|------|
|Decent. Games play at 1080p or lower at medium-to-low settings. | Budget | **Nvidia**: GeForce GTX 1650 Super, GTX 1650. **AMD**: Radeon RX 6500 XT, RX 6400, RX 5500 XT 4GB/8GB. |  
| Standard. Games play at 1080p at medium-to-high settings. | Mid-Range | **Nvidia**: GeForce RTX 3050, RTX 2060, GTX 1660 Ti, GTX 1660 Super, GTX 1660. **AMD**: Radeon RX 6600 XT, RX 6600, RX 5700, RX 5600 XT. |
| Great. Games play at 1440p or 1080p w/ 144Hz refresh rate at high-to-ultra settings. | High-End | **Nvidia**: GeForce RTX 3070 Ti, RTX 3070, RTX 3060 Ti, RTX 3060, RTX 2080 Ti, RTX 2080 Super, RTX 2070 Super, RTX 2070, RTX 2060 Super. **AMD**: Radeon RX 6800, RX 5700 XT. |
| Premium. Support 4k, new ray-tracing and AI technology. | Premium/Extreme | **Nvidia**: GeForce RTX 3090 Ti, RTX 3090, RTX 3080 Ti, RTX 3080, Titan RTX. **AMD**: Radeon RX 6900 XT, RX 6800 XT. |


### Storage
![ssd](./assets/images/ssd.png){: style="width:10em"}

The PC's storage drive is where the operating system (OS) is installed and files are kept. The file system is what the OS uses to control how data is stored and retrieved. By separating data into pieces and giving each piece a name, the data is easily isolated and identified.

#### Storage Comparison

| Hard Disk Drive (HDD) | Solid State Drive (SSD) | m.2 Drive (m.2) |
|-----|-----|------|
| Low Cost | High Cost| High Cost |
| Mechanical Parts | No Mechanical Parts | No Mechanical Parts |
| Needs Power and SATA Data Cables | Needs Power and SATA Data Cables | Uses PCI-e Port on Motherboard (No Cables) |
| Slow Read/Write Speeds | Fast Read/Write Speeds | Fast Read/Write Speeds |

### PSU - Power Supply
![psu](./assets/images/psu.png){: style="width:15em"}

Power supply is important when building a PC, as it converts AC power into DC power for the CPU, motherboard, graphics card, and all peripherals. General guidelines are as follows:

- 500-600 Watts for a PC using the web and office apps.
- 650-850 Watts for a PC using any external GPU.

    !!! help "Unsure?"
        Check the GPU's power requirements for exact measurements.

#### Energy Efficiency
The 80 Plus certification program for power supply units offers 80 Plus, 80 Plus Bronze, 80 Plus Silver, 80 Plus Gold, 80 Plus Platinum and 80 Plus Titanium certification levels. The most efficient (and most expensive) Titanium tier offers more than 90% energy efficiency.

#### Power Supply Design
There are three types of PSUs on the market: Full Modular, Semi Modular, and Non Modular. Below is a table covering the different pros and cons between them.

| | Full Modular| Semi Modular | Non Modular|
|----|----|----|----|
|Air Flow | Excellent air flow due to less cable clutter | Good air flow with good cable management | Bad air flow due to cable clutter |
| Temperature | Low temperature reading due to less cable clutter | Fine temperature reading due to good air flow and cable management | Poor cable management will result in high temperature |
|Aesthetics | Easy to organize and manage for good looks | Good looks with decent cable management | Messy looks due to too many cables|
|Convenience | Convenient PSU replacement | Easier PSU replacement with less cables to unplug | Need to remove all cables when switching PSU |
|Customization | Can be fully customized | Limited customization options | No customization options |

!!! warning
    If a motherboard that supports overclocking is purchased, it may require dual ATX 8 pin or 8+4 pin for the CPU. Check to make sure the selected power supply has them.

### Case
![case](./assets/images/case.png){: style="width:9em"}

Selecting a case can be done mostly to personal taste, but there are a few factors to keep in mind.

- The case needs to have good air flow, so there should be lots of fan mounting spots. Look for wide openings at the front for air to enter, and having them filtered will help keep dust out of the case.
- Check what size motherboard the case will accept, most motherboards are ATX sized and won't fit in smaller cases.
- Check the length of GPU the case accepts, as newer graphics cards can reach 27-33cm in length.
- Check the case for mounting spots for all storage devices.
- For air cooling, check the case's maximum CPU cooling height in millimeters, having at least a few mm more than the height of the actual cooler.
- For liquid cooling, the radiator needs a spot to mount to the case, so check for 240 or 360mm radiator mounting locations at the front or the top. The top is the recommended location for keeping the inside of the case cool as the radiator will exhaust directly outside the case.

    !!! danger
        **Never** mount the radiator to the bottom of the case. The pump should never be at the very top of a liquid loop as the small amount of air in the loop will want to pool there, reducing the efficiency of the CPU cold-plate and pump.

- Tempered glass panels show off the internals but add considerable weight, and care must be taken when transporting and after installation. Be cautious not to torque fasteners too tightly on the glass as over time this can cause it to shatter.

## Operating Systems
An operating system is considered to be the backbone of any system. Without an operating system, the user and system cannot interact. The three most universally used operating systems are: Windows, MacOS, and Linux.

- **Windows** is developed by Microsoft and is comparatively the most accessible operating system on the market.
- **MacOS** is developed by Apple for their Macintosh systems and is geared towards users that want performance fused with simplicity.
- **Linux** is a free, open-source family of operating systems initially developed by Linus Torvalds and currently updated by the GNU Project and the Linux community. It is mainly used by enthusiasts and companies that run servers and applications with the need of high security and no downtime.
