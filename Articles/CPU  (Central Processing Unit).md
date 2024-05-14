One key component of any computer is a CPU. A CPU (or processor) is the brains of your computer; it runs applications from calculators, web browsers, to video games. However, a computer is more than just a CPU. CPUs handle the calculations that allow us to run code, but they must work without other hardware components such as [[Memory]] and graphic processing units (GPUs) to function as the computers we know today.

![[cpu2.png]]

---
#### CPUs

A CPU consists of billions of microscopic [[Transistors|transistors]] that together handle instructions in the form of 0s and 1s. These instructions are prescribed by humans in the form of code, and so by writing code, we can tell a computer to do whatever we want it to do.

A CPU’s tasks can be broken into four main steps: fetch, decode, execute, and store. Fetching is the process of getting instructions from some location in memory, decoding is translating those instructions into something the CPU can directly understand, executing is actually following the given instructions, and storing is saving the result of the execution somewhere for later access. CPUs go through this overall process many, many times.

![[cpu1.png]]

CPUs are organized into cores, or parts of the CPU that can independently process instructions. Early CPUs only had one core, however, today’s computers often have multiple; you’ll often find computers that advertise dual and quad-core processors. Each core can only run one program at a time. For example, if you only have one washing machine, you can only run one load of laundry at a time. If you have multiple loads of laundry, you would have to wait until the previous load is finished before washing the next. Having multiple cores is like having multiple washing machines. By leveraging multiple cores within a CPU, computers are able to multitask and run multiple things at once.

In addition to having multiple physical cores, CPUs can utilize a technology called hyperthreading. Hyperthreading allows a single physical core to act as two individual cores. These new cores are known as virtual cores because they aren’t actually cores, but computer software treats them as if they are. Virtual cores can be used to speed up programs, however they are not as advantageous as physical cores.

---
#### SOC- System on a Chip

CPUs do not work alone. In order for CPUs to work with other things, CPUs are usually connected to a [[Motherboard]], the main circuit board that connects all of a computer’s hardware components. However, motherboards with its hardware components can be quite large. While modern desktops and laptops still have CPUs connected to a larger motherboard, smaller devices like smartphones and tablets take advantage of something called system on a chip (SoC).

A SoC is exactly what it sounds like: it is an entire system on a single chip. In a SoC, the CPU is fully integrated with memory, GPUs, and more on a single chip. You can think of it as fully functional computer in a tiny, tiny box. SoCs are significantly smaller and require less power than traditional CPUs, but there is a tradeoff. By nature of having a tightly integrated unit, SoCs are inflexible and cannot be customized or upgraded. In other words, if part of the SoC breaks, the whole things breaks, and there is no way to improve or replace any of its components.

Here are some examples of Systems on a Chip:
- Popular in phones, tables, and game consoles
	- Apple M1
- Raspberry Pi
- Arduino devices

![[raspberrypi1.png]]
*Raspberry Pi*

![[soc1.png]]
*System on a Chip*

---
#### Notes

  * The first general purpose, commercially available, programmable CPU was developed by Intel in 1971
	  * Intel 4004
	  * 2,300 transistors

<hr>

**<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">QUESTIONS</span>**

<details>
	<summary>Critical Thinking! Does every computer need a CPU? Why or why not?</summary>
		<p style="font-style: italic">Yes! If it doesn't have a CPU, its not a computer.</p>
</details>

<hr>

<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

CPUs have been getting smaller and more powerful every year for decades. In fact, this progression is so predictable that it has a name; Moore's Law. Read about [Moore's Law](https://en.wikipedia.org/wiki/Moore%27s_law) here to learn more about the progression of CPU computational power over time.

<hr>

<span style="color: #7b6cd9; border: 2px solid #7b6cd9; padding: 3px">ACTIVITY</span>

On a Windows computer, you can check the current status of your CPU using the Windows Task Manager. Open your task manager and navigate to the "Performance" tab to view information about your CPU including speed and usage percentage.

![[taskmanager1.png]]

---
#### Related Articles

[[CPU  (Central Processing Unit)]]
[[Binary]]
[[Data]]
[[Motherboard]]
[[Computer Hardware]]
[[Transistors]]


