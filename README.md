# cs7639-o01-project-3--crazyflie-design-and-analysis-using-aadl-2025-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/cs7639-o01-project-3-crazyflie-design-and-analysis-using-aadl-2025-solved/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;132171&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS7639-O01  Project #3 -Crazyflie design and analysis using AADL 2025 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
CS-7639-O01 Project#3

Crazyflie design and analysis using AADL

About this project

For this project, we aim at using AADL to analyze an existing design of a small UAV, the Crazyflie, and then to extend it to add new capabilities.

This project is organized in multiple parts:

<ul>
<li>Part 0 is an introduction to AADL and toolchain. It is provided as a reference;</li>
<li>Part 1 is a walkthrough of the provided Crazyflie model, where you’ll perform multiple analysis and then expand the model;</li>
<li>Part 2 revisits the Crazyflie models, with the objective to perform safety analysis.</li>
</ul>
Deliverables

Part 1

<ul>
<li>A PDF report with answers to questions</li>
<li>A .zip archive with updated models</li>
</ul>
Part 2

<ul>
<li>A PDF report with answers to questions</li>
<li>A .zip archive with updated models</li>
</ul>
CS-7639-O01 – Project #3 Crazyflie design and analysis using AADL

&nbsp;

<h1>PART 0 – AADL LANGUAGE AND TOOLCHAIN</h1>
&nbsp;

In this part, we introduce the basic elements of the AADL Language and its toolchain.

&nbsp;

Suggested reading:&nbsp; the following provide a comprehensive first reference to the AADL:

<ul>
<li>Julien Delange, AADL in Practice, <u>http://aadl-book.com</u></li>
<li>John J. Hudak, Peter H. Feiler, <u>Developing AADL Models for Control Systems: A</u> <u>Practitioner’s Guide</u>, Software Engineering Institute (SEI) Technical Report CMU/SEI2007-TR-014, July 2007.</li>
</ul>
&nbsp;

<h2>1. About AADL</h2>
&nbsp;

The “Architecture Analysis and Design Language” (AADL) is both a textual and graphical language for model-based engineering of embedded real-time systems. AADL is used to design and analyze software and hardware architectures of embedded real-time systems.

The AADL allows for the description of both software and hardware parts of a system. It focuses on the definition of clear block interfaces, and separates the implementations from these interfaces. From the separate description of these blocks, one can build an assembly of blocks that represent the full system. To take into account the multiple ways to connect components, the AADL defines different connection patterns: subcomponent, connection, and binding.

An AADL model can incorporate non-architectural elements: non-functional properties (execution time, memory footprint, . . .), behavioral or fault descriptions. Hence it is possible to use AADL as a backbone to describe all the aspects of a system. Let us review these elements:

An AADL description is made of components. Each component category describes wellidentified elements of the actual architecture, using the same vocabulary of system or software engineering. The AADL standard defines software components (data, thread, thread group, subprogram, process) and execution platform components (memory, bus, processor, device, virtual processor, virtual bus) and hybrid components (system) or imprecise (abstract).

Component declarations have to be instantiated into subcomponents of other components in order to model architecture. At the top-level, a system contains all the component instances. Most components can have subcomponents, so that an AADL description is hierarchical. A complete AADL description must provide a top-most system that will contain certain kind of components (processor, process, bus, device, abstract and memory), thus providing the root of the architecture tree. The architecture in itself is the instantiation of this system, which is called the root system.

The interface of a component is called component type. It provides features (e.g. communication ports). Components communicate one with another by connecting their CS-7639-O01 – Project #3 Crazyflie design and analysis using AADL

features. To a given component type correspond zero or several implementations. Each of them describes the internal structure of the components: subcomponents, connections between those subcomponents. They can also refine non- functional properties, or add new ones.

The AADL defines the notion of properties. They model non-functional properties that can be attached to model elements (components, connections, features, instances, etc.). Properties are typed at- tributes that specify constraints or characteristics that apply to the elements of the architecture such as clock frequency of a processor, execution time of a thread, bandwidth of a bus. Some standard properties are defined, e.g. for timing aspects; but it is possible to define new properties for different analysis (e.g. to define particular security policies). Besides, the language is defined by a companion standard document that defines legality rules for component assemblies, its static and execution semantics.

The Figure 1 illustrates a complete space system, used as a demonstrator during the ASSERT project. It illustrates how software and hardware concerns can be separately developed and then combined in a complete model.

&nbsp;

&nbsp;

<em>Figure 1 AADL Assert Demonstrator </em>

<h2>2. About AADL toolchain</h2>
&nbsp;

The correct engineering of Cyber Physical Systems entails the designer to perform multiple types of analysis on a candidate architecture.

&nbsp;

<ul>
<li>Semantic analysis: is the model correct w.r.t. to basic concerns? e.g. interfaces, containment hierarchy, consistency of configuration parameters, etc.;</li>
<li>Timing analysis: a model captures functional chain, and end-to-end flow path for data. One may want to assess if a given time budget allocated to each function is sufficient to support the system capabilities;</li>
</ul>
&nbsp;

CS-7639-O01 – Project #3 Crazyflie design and analysis using AADL

<ul>
<li>Scheduling analysis: at a later stage of refinement, one may want to ensure the low-level architectures (threads, buffers, etc.) are correctly configured so as to support all timing requirements;</li>
<li>Safety analysis: are the failures modes correctly defined? handled?</li>
</ul>
To support these analyses, we will use OSATE, from <u>http://osate.org</u>, developed by CMU/SEI. This is the reference implementation of an AADL toolchain. It supports text or graphical editing, timing and safety analysis;

<ol start="3">
<li>Using a virtual machine [recommended]</li>
</ol>
A virtual machine is provided with all the tools (see section 4 below). It is available at the address: https://drive.google.com/file/d/1oN9hWWVP9ocj3gKWPhRiVrDr0sUcU08L/view? usp=sharing login: cs7639 / password: pqsszd

To open the ova file,

<ol>
<li>download the ova file to your computer</li>
<li>install VMWare Workstation (<u>https://www.vmware.com/ products/workstation-player.html</u>)</li>
<li>open the ova file with VMWare using the default settings Make sure you read the readme file on the desktop of the VM.</li>
<li>Installation of the toolchain on your own machine</li>
</ol>
It is expected you can install all tools on a laptop in less than 1.5 hours. Simply refer to each web site for details. We strongly suggest you opt for a Linux-based installation.

<ul>
<li>Download OSATE from <u>http://osate.org/osate-releases.html#stable-releases</u></li>
<li>Install Cheddar plug-in: go in Help -&gt; Install Additional OSATE Components, and Cheddar from <u>http://beru.univ-brest.fr/cheddar/</u></li>
</ul>
<ol start="5">
<li>Project models</li>
</ol>
For this homework and the future project, we will use the AADL models from the following repository: <u>https://github.com/OpenAADL/Crazyflie</u>

It is advised you clone the repository, this would allow for future updates of the models.

The project files have been setup already in the virtual machine provided.

CS-7639-O01 – Project #3 Crazyflie design and analysis using AADL

<h2>6. Guided tour of the tools</h2>
&nbsp;

<h3>a. OSATE</h3>
&nbsp;

<em>[ Note that OSATE is updated regularly, some modifications on the GUI have been done recently. The following text is compatible with OSATE2.4.0.&nbsp; ] </em>

&nbsp;

<ul>
<li>Start OSATE.</li>
</ul>
&nbsp;

The workspace is organized using regular conventions of IDE:

<ul>
<li>The left panel is the list of files,</li>
<li>The central panel the current model/file being edited,</li>
<li>The right panel is the outline, with the list of model entities (system, thread, process, etc.).</li>
</ul>
&nbsp;

<ul>
<li>To update the repository: right click on the Crazyflie project in the left panel, then select Team -&gt; Pull</li>
</ul>
&nbsp;

<ul>
<li>To view graphical models corresponding to textual ones, you may either open files from the diagrams folder, or right-click on a model element in the outline panel, and click on “Open Diagram”.</li>
</ul>
&nbsp;

Note: some graphical models have been built and organized, some others not. Expect some obfuscated diagrams.

&nbsp;

Note #2: a right-click on the diagram allows to select elements that will be visible. Some properties, connections might not be visible immediately.

&nbsp;

&nbsp;

&nbsp;

<ul>
<li>To analyze a model, one has to identify the “root” of the system. The root is defined as the top-most component of a model from the outline (right panel). We have two root systems:
<ul>
<li>Impl, in crazyflie_functional.aadl o Crazyflie_System.Impl, in crazyflie_system.aadl</li>
</ul>
</li>
</ul>
&nbsp;

Analyzing an AADL model is a two-step process:

<ol>
<li>Instantiate the root system: in the right panel that lists all components, rightclick on the top-most system implementation (i.e. System Crazyflie_System.impl) and select instantiate.</li>
</ol>
This will generate a .aaxl2 file in the models/instances directory

<ol start="2">
<li>Perform the analysis: right click on the generated file, and select the analysis from the AADL Analyses menu.</li>
<li>For Cheddar, select the instance file, then the “Cheese” icon in the main menu bar to generate the Cheddar XML file. Then run Cheddar</li>
</ol>
&nbsp;

Supported analyses are: o Safety –&gt; Run Fault Tree Analysis / Fault Impact Analyses

<ul>
<li>Timing –&gt; Check Flow Latency</li>
<li>Scheduling Analysis (using Cheddar)</li>
</ul>
&nbsp;

CS-7639-O01 – Project #3 Crazyflie design and analysis using AADL

<h1>PART 1 – Unboxing the Crazyflie</h1>
About the Crazyflie UAV

The Crazyflie 2.0 is a versatile flying development platform that weighs only 27g and fits in the palm of your hand.

The Crazyflie 2.0 is an open source project, with source code and hardware design both documented and available. All information is available from BitCraze.io website: <u>https://www.bitcraze.io/crazyflie-2/</u>.

Crazyflie 2.0 System Architecture<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>

Crazyflie 2.0 is architectured around 2 microcontrollers:

<ul>
<li>A <strong>NRF51</strong>, Cortex-M0, that handles radio communication and power management:</li>
<li>ON/OFF logic</li>
<li>Enabling power to the rest of the system (STM32, sensors and expansion board)</li>
<li>Battery charging management and voltage measurement</li>
<li>Master radio bootloader</li>
<li>Radio and BLE communication</li>
<li>Detect and check installed expansion boards</li>
<li>An <strong>STM32F405</strong>, Cortex-M4@160MHz, that handles the heavy work of flight control and everything else:</li>
<li>Sensor reading and motor control</li>
<li>Flight control</li>
<li>Telemetry (including the battery voltage)</li>
<li>Additional user development</li>
</ul>
See Figure 2 for more details.

The nRF51822

The two main tasks for the nRF51 is to handle the radio communication and the power management. It acts as a radio bridge (it communicates raw data packet to the STM).

Crazyflie 2.0 use the radio for both CRTP and BLE, but the hardware also supports other protocols like ANT. The CRTP mode is compatible with the Crazyradio USB dongle and it provides a 2Mbit/seconds data link with low latency. Test shows that the latency of the radio link is between 360us and 1.26ms, at 2Mbps without retry and a packet size of respectively 1 and 32 bytes. The minimum achievable latency with Bluetooth is 7.5ms but current implementation is more around 20ms. The main benefit of the CRTP link with the Crazyradio is that it’s easily implemented on any system that supports USB host which, makes it the first choice to hack and experiment with the Crazyflie. BLE is implemented mostly with the use case of controlling the Crazyflie 2.0 from a mobile device.

One of the other particularities of the nRF51 chip is that it was designed to run from a coin battery, which means that it is pretty well suited for low energy operation. So, the NRF51 is also responsible

for power management. It handles the ON/OFF logic which means that the NRF51 is always powered and that different action are possible when pressing the ON/OFF button for a long time (i.e. this is used to start the bootloader). It is also possible to wake Crazyflie 2 from one pin of the expansion port, which allows wake-up by an external source.

&nbsp;

<em>Figure 2 Crazyflie 2.0 system architecture </em>

<h2>The STM32F405</h2>
The STM32 runs the main firmware. Even though it is started by the NRF51, it acts as a master towards the NRF51. It implements flight control, and all communication algorithm. The expansion port is mainly connected to the STM32 so the driver for expansion boards sits in the STM as well.

The STM32F405 has 196kB of RAM which should be enough for anyone (famous last words…). This is overkill for just the flight controller but it allows for more computationally intensive algorithms, for example sensor fusion between inertial sensors and the GPS data.

<h2>Inter-MCU communication</h2>
The communication between the two CPUs is handled by the syslink protocol. It is a simple packetbased protocol we made to have an extensible communication scheme.

Syslink provides messages for carrying all required communication between the CPUs. The STM32 is the master and the NRF51 the slave. As much as possible we try to keep the NRF51 simple and stupid to offload complex algorithm in the STM32.

Example of syslink message are:

<ul>
<li>Raw radio packets, to be sent and received</li>
<li>Power management measurement</li>
</ul>
&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

<h2>Crazyflie 2.0 Controller architecture<a href="#_ftn2" name="_ftnref2"><sup>[2]</sup></a></h2>
&nbsp;

The following images illustrate the architecture of the controller at system-level and implementation levels. The controller is split in two sub-controllers: one Attitude PI-Controller running at 250Hz, and one Rate P-Controller running at 500Hz.

&nbsp;

<em>Note: the detail of the controllers is outside the scope of the assignments. </em>

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

<h2>AADL modeling of the Crazyflie</h2>
&nbsp;

We built a set of AADL models to serve as an entry point for our project. The models are both graphical and textual, they are organized as follows:

&nbsp;

<ul>
<li>aadl: abstract functional chain of the Crazyflie, adapted from the functional architecture</li>
<li>aadl: hardware part of the UAV, capturing the various hardware elements.</li>
<li>aadl: software part of the UAV, it is a candidate implementation only</li>
<li>aadl: list AADL data types used for the component interfaces ;</li>
<li>aadl : one candidate full system, combining the hardware and software elements;</li>
<li>aadl : mapping of the abstract functional chain to the candidate implementation.</li>
</ul>
&nbsp;

These models capture the outcome of a typical design flow for CPS.

<ul>
<li>First, we built the high-level functional chain (aadl),</li>
<li>Then, we built the hardware (aadl) and software (crazyflie_software.aadl) candidates and one system combining them (crazyflie_system.aadl). By combining, we mean that the software elements are mapped to hardware ones.</li>
<li>Later, we built the crazyflie_final model to ensure all functions are bound to implementation elements.</li>
</ul>
&nbsp;

<em>Note: the provided models are starting elements for the next steps of the project only! You may only assume they can be opened by the various tools. </em><em>&nbsp;</em>

<h2>Part 1.1: Flow latency analysis</h2>
&nbsp;

<em>Note: in this part, we will use OSATE to analyze and extend the model. </em>

&nbsp;

Suggested reading:

<em>“Impact of Runtime Architectures on Control System Stability” by</em> Peter H. Feiler and Jürgen

Hansson, ERTS2008, &nbsp;&nbsp;<u>https://hal-insu.archives-ouvertes.fr/insu-02270102</u>

&nbsp;

The proposed model has a few flows modeled through the system. In AADL, a flow captures the propagation of data and its processing by various model elements such as devices and threads. Flows are an interesting capability to model expected end-to-end latency in processing chain. Our CrazyFlie UAV has multiple paths from sensors to actuators, and it would be beneficial to review them all.

&nbsp;

In AADL, a flow is a piecewise definition of data “flowing” through component interfaces. The root of a flow is an “end to end flow” that lists its constituent, or atomic flow.

&nbsp;

Here is the definition of one end-to-end flow from the Crazyflie_System package:

&nbsp;

flows

— etef1 represents the functional chain from MPU9250 IMU to STM32 &nbsp;&nbsp;&nbsp;&nbsp;— firmware to one of the propeller.

&nbsp;

etef1 : end to end flow MPU9250.f1 -&gt; C11 -&gt; STM32F405_Firmware.f2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -&gt; C12 -&gt; M1.f1 { latency =&gt; 0 ms .. 2 ms;};

&nbsp;

Each subcomponent (MPU9250, STM32F405_Firmware, etc.) lists additional flow, here f1 and f2 respectively. An end-to-end flow starts with a flow source (e.g. a sensor) and ends with a flow end (e.g. an actuator)

&nbsp;

<strong>Q1:</strong> In your report, list all existing end-to-end flows in the existing AADL model (system and functional), and propose additional flows that may be missing. You will justify their inclusion and the associated configuration parameters.

&nbsp;

<strong>Q2: </strong>add the additional end-to-end flows from Q1 in the AADL models, as well as necessary flow source/path/sink.

&nbsp;

For each of them, you’ll use specific notation to indicate the modified elements. Suggested annotation is to use AADL comments, like

&nbsp;

—&nbsp; John <u>Doe</u> begin of addition for question Q2

—&nbsp; John <u>Doe</u> end of addition for question Q2

&nbsp;

where John Doe is changed to your actual name, and question adjusted accordingly.

&nbsp;

<strong>Q3:</strong> Execute the latency analysis on the instantiated model with the default settings. What do you observe on the obtained values?

&nbsp;

Considering that the Crazyflie has a symmetrical mechanical design, can you consider that some of the flows are redundant, i.e. capture the same behavior? Remember that flows measure the latency, not the value, of a signal.

<strong>&nbsp;</strong>

<strong>Q4:</strong> In the description of the Crazyflie architecture, the latency requirements for various aspects of the system are detailed (see figures page 9). You should convert the frequency to period. List, if any, the end-to-end flows that these requirements affect. How will the end-to-end latency for these flows be affected by the requirements? Does the current architecture meet these requirements? If not, which end-to-end flows need additional timing allocation?

&nbsp;

<h2>Part 1.2 Simulation of the model</h2>
&nbsp;

<em>Note: in this part, we will use Cheddar to simulate the Crazyflie_System model.&nbsp; </em>

&nbsp;

A typical error when building models is lacking ways to “debug” your system. Simulation is one possible option to address this issue.

&nbsp;

Cheddar proposes a simulator that will exploit scheduling information from tasks and devices.&nbsp; For instance, the following indicates that every 10ms this device will output some data through the DOF6 port. Later on, we may infer the bus used for this communication.

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

device MPU9250&nbsp;&nbsp; features

DOF6 : out data port Crazyflie_Types::Six_Axis.impl;&nbsp;&nbsp;&nbsp;&nbsp; i2c_bus : requires bus access Buses::I2C::I2C.impl;

&nbsp;

properties

Dispatch_Protocol =&gt; Periodic;

Period&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; =&gt; 10 ms;

&nbsp;

Another example is the definition of this thread:

&nbsp;

thread Power_Management

properties &nbsp;&nbsp;&nbsp;&nbsp;Priority =&gt; 2;

Dispatch_Protocol =&gt; Periodic;

Period =&gt; 500 us;

Compute_Execution_Time =&gt; 10 us .. 20 us;&nbsp;&nbsp; end Power_Management;

&nbsp;

The Compute_Execution_Time defines an interval for the time necessary to execute this thread. By construction, we assume that the deadline of an execution is equal to the period of the component.

&nbsp;

In this model, we use two dispatch protocols:

<ul>
<li>Periodic: the component will be executed periodically</li>
<li>Sporadic: the component will be executed only if an event is received on one of its <strong>event</strong> (data) <strong>port</strong>, and after some time elapsed represented by the Period property.</li>
</ul>
&nbsp;

<strong>Q5:</strong> simulate the model in Cheddar by loading the .xmlv3 file in the cheddar_models folder (generated from the system instance file by clicking the “Cheese” button in Osate) and clicking the green play button in Cheddar. To see the complete Gantt chart, you might need to readjust the Gantt chart panel size by dragging down the panel divider and zoom out. Are all threads executed? Does the execution match the behavior you expected for this system? In particular, you want to assess whether all ports are correctly dimensioned, if a thread may miss its deadline, etc. If something seems wrong, propose a correction. Note that there is no need to correct anything regarding the latency exceeding bound errors.

&nbsp;

<h2>Part 1.3 Scheduling analysis of the model</h2>
<strong>&nbsp;</strong>

In this part, we continue exploring the analysis of the model with Cheddar.

&nbsp;

Scheduling analysis provides a mechanism to assess schedulability of a system. Cheddar has multiple plug-ins to perform scheduling analysis.

&nbsp;

<strong>Q6:</strong> run scheduling analysis on the system by clicking the gear button, what can you conclude?

&nbsp;

<strong>Q7:</strong> how would you relate flow analysis, simulation and scheduling analysis? What is their benefit in a complete Systems Engineering process?

&nbsp;

<h2>Part 1.4 Adding new component: Flow Deck</h2>
&nbsp;

This page: <u>https://wiki.bitcraze.io/projects:crazyflie2:expansionboards:flow</u> lists an expansion board for the CrazyFlie. In order to improve the maneuverability of the UAV, one needs to add an additional sensor to evaluate lateral movement of the UAV. This solves the “sliding” behavior of the drone, at the expanse of extended computation.

In this part, we want to add the Flow Deck expansion board to the initial model.

&nbsp;

One strategy is to define the corresponding devices in the hardware package, and add them to the hardware system, and add related model blocks to the software and functional models.

&nbsp;

To avoid losing the previous model, we want to use the refinement/extension capabilities of AADL to add elements related to the Flow Deck expansion board.

&nbsp;

You may review this example, from Crazyflie_System

&nbsp;

system implementation Crazyflie_System.impl&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; extends Crazyflie_Hardware::Crazyflie.impl

subcomponents

nRF51822_Firmware : process Crazyflie_Software::nRF51822_Firmware;&nbsp;&nbsp;&nbsp;&nbsp; STM32F405_Firmware : process Crazyflie_Software::STM32F405_Firmware.impl;

&nbsp;

Here, we extend the hardware part and add software elements. A similar strategy may be deployed to add Flow Deck related elements.

&nbsp;

<strong>Q8:</strong> provide an expanded model with the Flow Deck integrated. Ensure all previous analysis are still feasible. You’ll provide the rationale for all the updates you performed in your report.

&nbsp;

&nbsp;

<h1>PART 2 – Safety Analysis</h1>
&nbsp;

In this part, we will evaluate the safety architecture of the UAV through multiple analysis mandated by the ARP4761 standard.

&nbsp;

Additional reading:

[1] Julien Delange, Peter H. Feiler, David P. Gluch, John J. Hudak, “<em>AADL Fault Modeling and Analysis Within an ARP4761 Safety Assessment</em>”. This report explains how to leverage the Error-Model version 2 to follow the ARP4761 safety process.&nbsp; The full report is available as SEI Technical Report from

<u>http://resources.sei.cmu.edu/library/asset-view.cfm?assetID=311884</u>

&nbsp;

This document lists in section 1 and 2 how to map AADL to analysis that are mandated by the ARP4761 safety process. This process is part of the many steps to create a certified system. In the following, we will apply some safety analysis to the Crazyflie model.

&nbsp;

<strong><em>Important Notes:&nbsp; </em></strong>

<ol>
<li><strong><em>you may either extend the models you created for part 1, or reuse the initial model and extend it. State clearly your option in your report. </em></strong></li>
<li><strong><em>to ease the modeling part of this project, you may add elements to existing components instead of using the extends/refines mechanism of AADL. In the following, we provide increments to be added to the model </em></strong></li>
</ol>
<strong><em>&nbsp;</em></strong>

<h2>Functional Hazard Analysis of the functional chain</h2>
&nbsp;

An FHA is a systematic examination of functions to identify and classify failure conditions of those functions according to their severity. The AADL Error Model Annex supports the FHA through property assignments within an AADL architecture model.

&nbsp;

Users can generate an FHA report using the Error Model Annex and OSATE, by assigning Hazard, Likelihood, and Severity property values to points of failure. Then, OSATE can generate the FHA report.

&nbsp;

The EMV2 is an annex language, it adds a set of new concepts and associated language elements to the model.

&nbsp;

The Crazyflie_Errors package defines a set of error types that can be propagated:

ValueError, ValueErroneous and Lost.

<ul>
<li>ValueError indicate the value cannot be produced;</li>
<li>ValueErroneous indicates an incorrect value has been produced;</li>
<li>Lost means the component is now defunct, and the associated function is lost.</li>
</ul>
&nbsp;

The Crazyflie_Errors package also defines an empty state machine, made of two states, Operational and Failed. This state machine will serve as a skeleton to build the failures modes of our UAV component.

&nbsp;

In the Crazyflie_Functional package, we built a first high-level view of the functional chain of our UAV. One may create an FHA from this functional chain, by attaching the identification of failure conditions. Keep in mind that at this level, we are purely descriptive.

&nbsp;

In the following example, we attach probability of occurrence of entering in the Failed mode, and some documentation attached to this faulty situation, in addition to its severity and likelihood. Section 2.10.1 of [1] provides a complete definition of the Hazards property.

&nbsp;

abstract Accelero&nbsp;&nbsp; features

Accelero_Out : out data port;

—&nbsp; [..]&nbsp;&nbsp;&nbsp; annex emv2 {**

use types Crazyflie_Errors;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — definition of error types&nbsp;&nbsp;&nbsp;&nbsp; use behavior Crazyflie_Errors::simple;&nbsp; — definition of error modes

properties

— Useful for FHA reports

EMV2::OccurrenceDistribution =&gt; [ ProbabilityValue =&gt; 1.0e-9 ;

Distribution =&gt; Poisson;] applies to Failed;

EMV2::severity =&gt; 1 applies to Failed;

EMV2::likelihood =&gt; C applies to Failed;

EMV2::hazards =&gt;

([ crossreference =&gt; “”;

failure =&gt; “Loss of sensor readings”; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;phases =&gt; (“all”);

description =&gt; “Sensor failure”;

comment =&gt; “May be critical as no redundancy on UAV”;

]) applies to Failed;

**};&nbsp;&nbsp; end Accelero;

&nbsp;

A typical issue when building this analysis is to get meaningful value for the probability of occurrence of errors for a component. OEMs usually do not publish them on a regular basis, except for military-grade ones<a href="#_ftn3" name="_ftnref3"><sup>[3]</sup></a>. Here, we assumed an unrealistic value of 10<sup>-9</sup>.

&nbsp;

<strong>Q9: </strong>Update Crazyflie_Functional::Crazyflie_Functional_Chain.impl and its subcomponents with EMV2 properties to support the FHA. You may adjust the hazards considering only failure of hardware (CPU, memory, sensors, etc.) or mechanical elements only. We consider, for the moment that the pilot and the software are defect free.

&nbsp;

<strong>Q10:</strong> Generate the corresponding FHA report using OSATE.

&nbsp;

Note: you’ll observe OSATE simply aggregates the elements from the model. The additional benefit is that the modeling language performs cross-check on the name of the failure modes, the coverage of modes etc. These ensure the report is consistent and complete.

&nbsp;

&nbsp;

&nbsp;

&nbsp;

<h2>Reliability Analysis of the functional chain</h2>
&nbsp;

After performing the FHA, one may wonder how reliable the system is. Fault Tree Analysis (FTA), leverages the architecture of the system to evaluate the failure probability of the system.

&nbsp;

To achieve this goal, one needs to capture the failure mode of the system as a composition of the failure mode of the system.

This can be captured in Crazyflie_Functional_Chain.impl using an EMV2 subclause and a composite error behavior. This behavior refined the error automata of the system with a Boolean equation stating when the system is either in Operational or Failed mode. Obviously, the system is in Operational mode when all sensors are Operational, but this is also incomplete.

&nbsp;

system implementation Crazyflie_Functional_Chain.impl

—&nbsp; [..]

annex EMV2 {**

use types Crazyflie_Errors;&nbsp;&nbsp;&nbsp;&nbsp; use behavior Crazyflie_Errors::simple;&nbsp;&nbsp;&nbsp;&nbsp; composite error behavior &nbsp;&nbsp;&nbsp;&nbsp;states

[ Acc.Operational&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and Gyro.Operational&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and Magneto.Operational

]-&gt; Operational;

[ TBD

]-&gt; Failed;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end composite;

**};

end Crazyflie_Functional_Chain.impl;

&nbsp;

<strong>Q11: </strong>What are the conditions for all elements to be either in the Operational or Failed modes? Extend the model accordingly. What is the failure probability you get, using the “Fault Tree Analysis” plug-in?

&nbsp;

<h2>Taking into account software “failure”</h2>
&nbsp;

<em>Note: the concept of software failure is source of eternal debate. Software fails in a reliable way through bugs, yet they may react “strangely” in case of physical bugs. In this section, we consider that software may propagate errors in all cases. </em>

&nbsp;

If one considers the Sensor_Fusion function, we can see it may receive error values, and propagate some. This notion of propagation of errors is strongly related to the concept of flows we explored in Part 1. This can be captured in the following way. Here, the Accelero device may send ValueError through its Accelero_Out feature:

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

&nbsp;

abstract Accelero

—&nbsp; [..]

annex emv2 {**

use types Crazyflie_Errors;

use behavior Crazyflie_Errors::simple;

error propagations&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — outgoing error propagation

Accelero_out: out propagation {ValueError};&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; flows

–When the sensor fails, its error is propagated through port Accelero_Out

ErrorSource: error source Accelero_out {ValueError} when {ValueError};

end propagations;

—&nbsp; [..]&nbsp;&nbsp;&nbsp;&nbsp; **};&nbsp;&nbsp; end Accelero;

<strong>&nbsp;</strong>

<strong>Q12: </strong>Update the model to capture all error sources (components) in the functional chain, using the Accelero abstract component as a template.

&nbsp;

The Sensor_Fusion abstract component is in charge of combining the inputs from the three sensors. It outputs one vector state that corresponds to the attitude of the UAV.

&nbsp;

In the following, we illustrate the additional elements one may add to capture the propagation of errors in the system:

<ul>
<li>the error propagations subclause captures the way error may enter (in) or exit (out) a block, the flows section indicates the relationships between inputs and outputs ports</li>
<li>the component error behavior captures the error automata of the system. The TBD part is a Boolean equation that captures how the system moves from the Operational to the Failed mode. The propagations part indicates the error being reported in case of an error.</li>
</ul>
&nbsp;

abstract Sensor_Fusion

—&nbsp; [..]

annex EMV2 {**

use types Crazyflie_Errors;

use behavior Crazyflie_Errors::simple;

&nbsp;

error propagations

Accelero_In : in propagation {ValueError};&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Data_F_Out&nbsp; : out propagation {ValueError};&nbsp;&nbsp;&nbsp; flows

f1 : error path Accelero_In -&gt; Data_F_Out;&nbsp;&nbsp;&nbsp; end propagations;

&nbsp;

component error behavior &nbsp;&nbsp;&nbsp;transitions

t1 : Operational -[TBD&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ]-&gt; Failed;&nbsp;&nbsp;&nbsp; propagations

Failed -[]-&gt; Data_F_Out{ValueError};&nbsp;&nbsp;&nbsp;&nbsp; end component;

**};&nbsp;&nbsp; end Sensor_Fusion;

&nbsp;

<strong>Q13:</strong> propose and implement an update to the model that captures the following hypothesis on the fusion algorithm used: any error as input will translate as an error as output.

<strong>&nbsp;</strong>

We may now consolidate all analysis

&nbsp;

<strong>Q14:</strong> run again the Fault Tree analysis, how does the value compare with the previous one? Is it expected?

&nbsp;

<strong>Q15:</strong> the fault impact analysis plug-in allows one to see how an error propagated in the functional chain. Execute the plug-in and compare the output to your model. How can you link each element of the fault impact analysis to model elements?

&nbsp;

<strong>Q16:</strong> for the moment, we mostly performed basic updates on the system. Complete the error model by adding failures on motors, and the propagation of error value through the controller.

<strong>&nbsp;</strong>

<strong>&nbsp;</strong>

<a href="#_ftnref1" name="_ftn1"><u>[1]</u></a><u> From </u>https://wiki.bitcraze.io/projects:crazyflie2:architecture:index<u>&nbsp; </u>

<a href="#_ftnref2" name="_ftn2"><u>[2]</u></a> <u>From </u>https://wiki.bitcraze.io/doc:crazyflie:dev:fimware:sensor_to_control<u>&nbsp; </u>

<a href="#_ftnref3" name="_ftn3"><u>[3]</u></a> https://emcore.com/products/sdi500-tactical-grade-imu-inertial-measurement-unit/<u>&nbsp; </u>
