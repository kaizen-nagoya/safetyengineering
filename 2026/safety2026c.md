Models, processes and services designed by source codes of safety system for mobility with LLM and MCP.

○	Dr. Kiyoshi Ogawa, Atec inc.		

1 Background
This paper is state of art in 2026 and examines the relationship between the use of generative AI for safety design in mobile devices and existing technologies. During this process, we will delve deeper into the relationship between the program’s source code and the model, process, and service. In the field of eco- nomics, the value of the agents in a transaction was expressed using a system of inequalities, representing the phenomenon known as equi- valent exchange.[1] In the field of engineering, I worked on porting a communication simulator that connects PCs and mainframes to improve the de- velopment environment[2], and for my graduation research, I performed the Pade approximation on simultaneous diﬀerential equations.[3] I ported VZ editor, an editor for MS-DOS, to the NEC N5200 oﬃce personal computer.[4]
(1) AUTOSAR Open Source Project
Before AUTOSAR’s specifications were oﬃcially released, I participated in a project to create open-source AUTOSAR at the request of an OEM. I was responsible for education and deputy head of quality and safety analysis. Because the specifications had not yet been released, we created the ISO OSEK/VDX OS as opensource software. ISO OSEK/VDX OS is equivalent to the ITRON automotive profile. In reality, it was ported from the ITRON JSP source code. I was res- ponsible for testing the open-source project for the ITRON Smallest Set Profile, which is equivalent to ISOOSEK/VDX’ OS BCC1. As a secretary of ISO/IEC JTC1 SC7, I participated in deliberations on the international standardization of UML. As a liaison oﬃcer from ISO/IEC JTC1 SC7 to ISO/IEC JTC1 SC22, I participated in discussions on improving the quality of the C language. As a liaison oﬃcer from ISO/IEC JTC1 SC7 to ISO/TC 22/SC 32, I participated in deliberations on ISO 26262. At the Yokohama conference, with the approval of the BMW representative who chaired SC32, I gave a presentation on the importance of HAZOP based on safety related vehicle system.
(2) Embedded Systems Core Engineer Training Project
Nagoya Institute of Technology and a parts manufacturer have developed an assembly language description of motor control based on modern control theory. I was asked to take on the role of project manager for the embedded systems core personnel project in the Chubu region, and I gave lectures at Gifu University and Nagoya Institute of Technology. I conducted demonstration experiments at Gifu University and taught an intensive summer course as a part-time graduate lecturer for 10 years.
(3) IPA/JAXA critical software symposium
As part of a business project for the Ministry of Economy, Trade and Industry, I provided guidance on the implementation of ISO 9000 quality management systems. In relation to the expansion of ISO 9000 into the software field, at the request of NTT and Mitsubishi Electric, I was appointed to the ISO/IEC 15504 Process Assessment standardization committee. When JAXA co-hosted WOCs with IPA, I was appointed as the program chair and asked to share aerospace expertise with the automotive industry and to discuss and improve it together. 
(4)  Safety Engineering Symposium
I was encouraged to present my findings at the Safety Engineering Symposium by a former Toshiba employee from the nuclear power division who had guided me on safety analysis in the AUTOSAR open-source project. 1Between 2006 and 2020, I presented about 20 papers at safety engineering symposia [7]

2 Model
In this section, model means concept models, design
models and operation models on mechanical, electrical, material and software systems.
(1) Social model
In social models, the opposite is often true depending on one’s perspective. If you don’t describe the viewpoints from three or more diﬀerent perspectives, the discussion can become muddled.
(2) Moter control
The motor design tool JMAG allows the use of LLM and MCP through integration with MATLAB and Simulink. To use LLM with JMAG, it is advisable to add MCP to JMAG.

3 Process
in this section process means human process and com-
puter process. Automation is the process of replacing
the work of a genius with a computer. Most tasks that
anyone can do have already been replaced by computers.
(1) Water fall
In the era of paper cards, programs were loaded sequentially into a mainframe at regular intervals for processing, a person had to compile the code every few hours. Logical errors would waste several hours. It was necessary to draw diagrams and input gra- mmatically correct programs. In two-party transactions, focusing on the aspects where the customer pays were one way to eﬃcient development. Whether these customer-funded aspects may be called requirements, specifications, or designs depends on the customer terminology. On mainframes, the CPU, OS, language, database, and network are pre-configured by the manufacturer. From an eﬃciency standpoint, opti- mizing the work for the aspects the customer or oneself deems worth investing in can yield reasonable results. Estimates were based on the assumptions of following the waterfall model, V-model process, etc., provided by the computer manufacturer.
(2) Agile
Since the advent of 32-bit CPU PCs, design, build, and
run have become tasks that can be completed by a person on a PC. The order in which these tasks are performed can be left to the individual’s abilities, and it has become known that designing in source code is particularly eﬃcient. Agile is based on almost the same ideas as those insights gained at that time.
(3) DEVOPS
LLM has become useful not only for designing and operation on the cloud by the same person, but also for automating collaborative work among multiple people something that was diﬃcult to achieve with traditional PCs from environment setup using Git and Docker to test operation. The generation of checkers and counter examples also achieves LLM refinement. DevSecOps and DevSafeOps should be harmonized.

4 Services
A service refers to anything where the output can be defined for each input, such as the processing of materials, the movement of people or materials, or the processing of information, rather than specifying the exact method of processing. Another term for this is ”processing in a dark box.” Through data-centric and service-oriented design, we aim to improve service quality using incident databases and ML pattern extraction.
(1) Mobility
Mobile machinery includes trains, automobiles, ships, aircraft, and satellites. The structure of mobile ma- chinery involves comprehensively designing, prototyp-
ing, and evaluating physical and chemical phenomena,
including the structure, function, performance, materi-
als, fuel, heat, and air resistance of the engine/motor.
(2) Safety system
In situations where humans are outside the hazard source, such as with manufacturing machinery, the principle of isolation is eﬀective. However, in moving objects where humans are inside the hazard source, the principle of isolation alone is insuﬃcient. It is crucial to design for transitions to relatively safer states in all possible scenarios.

5 Tools
Various tools, including CAD, CAM, and CAE, are used for design, prototyping, and evaluation.
(1) Misra C and CERTC
MISRA C will be restructured to adhere to the spirit
and principles of C, and detailed rules will be rebuilt to
correspond to each applicable version of the C language standard. Furthermore, the probability calculation of cases where deviation results in higher quality will be automated, reducing the unnecessary work of simply adhering to the rules. On Cert C, it automatically generates intrusion, hijacking, and jamming programs for each corresponding com- munication protocol,and uses them to identify vulnera- bilities. Based on these results, improvement support for CERT C/C++ are automatically generated.
(2) STARC RTL design style guide
By creating versions of the STARC RTL Design Style
guide other than Verilog HDL and VHLD, or by auto- matically converting them to Verilog HDL and VHDL,
we can fill in previously untouched areas.
(3) Model based software design guide
By applying the JMARG guide, we can automatically generate model inspection tools and create more detailed guide candidates.
(4). deep learning and quantum computing
We held a study session on deep learning. A steel com- pany used a tool that processes multiple models in par-
allel and compares the results to improve the control of
its rolling process. On quantum computing, we are considering using LLM to conduct a preliminary investigation comparing quantum computing algorithms with conventional optimization techniques in specific domains to determine which approach is more suitable for which task.
(5)  LLM and MCP
By extending MCP (Model context protocol) to other
CAD, CAM, and CAE software, the inter-tool integra-
tion between tools with LLM (Large language model)
capabilities, such as MATLAB, can be dramatically improved. Thiere is an introduction FPGA language generation using MATLAB.[11]
(6) UML
In safety-related systems, safety analysis is performed
using state transition diagrams, time series diagrams,
time-series diagrams, and methods such as FTA, FMEA, and HAZOP. On state machine diagrfam there are reports of significantly improved quality compared to conventional methods by automatically generating Promela code from a state transition diagram to control a color PS printer, verifying it with SPIN, and then generating C source code. On sequence diagram I’m exploring a method that automatically generates and selects candidate state transitions from a sequence using LLM, which is the reverse of generating sequences from state transitions like Uppaal. On timing diagram, in a project funded by the Ministry of Economy, Trade and Industry, we attempted to automatically generate EtherCAT-compatible control programs from timing charts. A system could be devised where a mechanical designer writes control instructions, and the source code is generated.

6 Issue
(1) Tool Integration
When integrating multiple tools, data and program
transfers may fail due to version diﬀerences. Even without specific errors, the methods for generating and verifying ways to detect security vulnerabilities and potential bugs become more sophisticated. iit may not be important to only improve the API schema and tool interfaces. By not using Wikipedia, it is possible to ensure bias, expertise, and accuracy. 
(2) Intellectual property
As patents and copyrighted works increase exponen- tially through automated generation, the eﬀort required to verify who owns the automatically generated intellectual property will become enormous.
(3) Balancing eﬃciency and safety
For general purpose tools like HAZOP, the use of LLM may eliminate the need for work eﬃciency improvements like STAMP and STPA.
(4) Hazard of LLM
Many LLMs are English-dependent and do not reflect
the logic of Asian cultures such as Chinese culture
(which uses Chinese characters, representing the majority ethnic group) or Indian culture, nor do they reflect the cultures of minority ethnic groups.
(5) Responsibility boundaries
Determining the boundaries of responsibility in the
event of an accident, and whether insurance for au-
tomatically generated data is feasible, are social chal-
lenges, just like those for autonomous driving.

7 Future works
The following tools are extended to establish security-
by-design and safety-by-design. On Event-B, Bosh was involved in the Event-B project. He once con- sidered whether automotive software design could be described using Event-B. The stepwise refinement of Event-B was a diﬃcult task, requiring only highly skilled programmers. He wanted to improve eﬃciency by having a generative AI generate several candidates.
On the CSP system developed by the recently deceased Hoare was so complex that only exceptionally skilled programmers could fully describe it. I want to try to overcome these traditional diﬃculties with generative. 
(1) Programming language
Both C and C++ share the same structure: they are freestanding (without POSIX) and hosted (with POSIX).　The goal is to unify the source code of the C and C++　compilers and generate the C and C++ specifications　from the source code. We are also considering extensions that would allow the use of templates and namespaces in C.
(2) Operating system
The source code for POSIX PSE51 and OSEK/VDX
OS will be unified, allowing specifications to be generated from the source code. Ideally, the Priority Ceiling protocol will be introduced to Linux, allowing the selection of a mode that does not cause deadlocks.

8 Conclusion
The extent to which we can entrust generative AI with
harmonizing various perspectives, and what needs to be checked, is constantly changing. 

References
[1] Graduation Thesis: Equivalent exchange research,
Kiyoshi Ogawa, 1982, Hose University.
[2] porting on emulator to Hitachi Computer on PC-
9801, Kiyoshi Ogawa, 1985, NIT.
[3] Graduation Thesis: Pade approximation for simul-
taneous diﬀerential equations, 1986, NIT.
[4] porting VZ editor to N5200, Kiyoshi Ogawa, 1991
[5] Testing and Verification for Embedded Linux using
NIST POSIX Test Suite, Akihiro Yamana, Naoki Saito, Kiyoshi Ogawa, 3WSQC, 2005 in German.
[6] 7th TOPPERS of the Year: Smallest Set Profile Kernel, Naoki Saito, Kiyoshi Ogawa, Akika Sugimoto.
[7] SESJ Kiyoshi Ogawa Paper lists. https://github. com/kaizen-nagoya/References/blob/main/2026saf.md 
[8] Unexpected identification using HAZOP in safety analysis, Kiyoshi Ogawa, Kazuo Kashiwabara,
Nobuaki Tanaka, JSAE2020 Spring
