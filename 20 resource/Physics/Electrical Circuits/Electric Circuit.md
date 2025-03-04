**What is an electric circuit?**
An electric circuit is defined as a collection of electrical elements interconnected in some way. They can also be otherwise called as *electrical network*

Now these electrical elements can be divided into two types:
## Types of Electrical Elements

### **Active Elements**
these are elements or components that supply energy. These are capable of **controlling voltages** to produce gain or switching action within a circuit. There are two kinds of sources:
- **Voltage Sources**
- **Current Sources**

> [!info] Note!
> It is important to note that all sources that are talked about in this note will refer to **ideal sources,** meaning sources that can perfectly maintain constant voltage or current under all conditions. These are actually only theoretical concepts made to make calculations simpler. **Unideal sources** on the other hand are real-world sources, as in reality, there are no sources that can perfectly maintain their voltage/current. Hence, these are sources that may be affected by its internal resistance, limited power supply, its efficiency, heat dissipation, and so on.


Now both voltage sources and current sources can either be independent or dependent / controlled sources. An **Independent Source** is able to deliver voltage or current regardless of the network connection and its sources are  typically represented as a circle in a circuit, *see next image*.

![[Pasted image 20250205005159 1.png| center]]

Meanwhile, **Dependent Sources** are sources that depend on a *controlling variable* connected in some other part of the network. This means that its value is dependent on another variable, varying and changing (i.e. its value is 2v, v is a variable value that can be derived from another component). It is typically represented by either an arrow or a diamond shape, *see next image*. 

![[Pasted image 20250205005417 1.png| center]]

Dependent sources can usually be seen when modeling elements such as transistors,
operational amplifiers, and integrated circuits. Here is an example of a circuit with a dependent source:

![[Pasted image 20250210123916 1.png| center]]

At first glance, it may seem that 10i would be 10 A, but this value is actually a voltage source and the value of 10 is dependent on the value of I which flows through the element C.

There are four possible types of dependent sources as follows:
- **A voltage-controlled voltage source (VCVS).**
- **A current-controlled voltage source (CCVS).**
- **A voltage-controlled current source (VCCS).**
- **A current-controlled current source (CCCS)**

### **Passive Elements**
these are elements that **cannot** supply energy. These elements strictly absorb or store energy. Here are examples of major and basic passive elements:
- [[Resistor]] - absorbs energy
- [[Inductor]] - stores energy
- [[Capacitor]] - stores energy
