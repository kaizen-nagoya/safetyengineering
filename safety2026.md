Models, processes and services designed by source codes of safety
system for mobility with LLM and MCP.
Dr. OGAWA Kiyoshi, Aetc. inc.
April 9, 2026

Abstract

This paper examines the relationship between the use
of generative AI for safety design in mobile devices
and existing technologies. During this process, we will
delve deeper into the relationship between the program’s
source code and the model, process, and service.
Regarding UML, I received guidance from the presi-
dent of SparkSystems Japan; for model-based develop-
ment, from Takayuki Kubo of Aisin AW at the time;
and for formal methods, from people at the National In-
stitute of Advanced Industrial Science and Technology
and Takeshi Hori of the Hokkaido Prefectural Industrial
Research Institute.

1 background
1.1 self introduction
In the field of economics, the value of the agents in a
transaction was expressed using a system of inequali-
ties, representing the phenomenon known as equivalent
exchange.[1] In the field of engineering, I worked on port-
ing a communication simulator that connects PCs and
mainframes to improve the development environment[2],
and for my graduation research, I performed the Pade
approximation on simultaneous diﬀerential equations.[3]
I ported VZ editor, an editor for MS-DOS, to the NEC
N5200 oﬃce personal computer.[4]
1.2 AUTOSAR Open Source Project
Before AUTOSAR’s specifications were oﬃcially re-
leased, I participated in a project to create open-source
AUTOSAR at the request of an OEM. I was responsi-
ble for education and deputy head of quality and safety
analysis. Because the specifications had not yet been
released, we created the ISO OSEK/VDX OS as open-
source software. ISO OSEK/VDX OS is equivalent
to the ITRON automotive profile. In reality, it was
ported from the ITRON JSP source code. Later, I
was responsible for testing the open-source project for
the ITRON Smallest Set Profile, which is equivalent to
ISOOSEK/VDX’ OS BCC1. As a secretary of ISO/IEC
JTC1 SC7, I participated in deliberations on the interna-
tional standardization of UML. As a liaison oﬃcer from
ISO/IEC JTC1 SC7 to ISO/IEC JTC1 SC22, I partic-
ipated in discussions on improving the quality of the C
language. As a liaison oﬃcer from ISO/IEC JTC1 SC7
to ISO/TC 22/SC 32, I participated in deliberations on
ISO 26262. At the Yokohama conference, with the ap-
proval of the BMW representative who chaired SC32
and the Bosch sector representative, I gave a presenta-
tion on the importance of HAZOP based on the AU-
TOSAR open source and JAXA/IPA WOCS initiatives.
1.3 Embedded Systems Core Engineer
Training Project
Nagoya Institute of Technology and a parts manufac-
turer have developed an assembly language description
of motor control based on modern control theory.[?] I
was asked to take on the role of project manager for
the embedded systems core personnel project in the
Chubu region, and I gave lectures at Gifu University and
Nagoya Institute of Technology.[?] I conducted demon-
stration experiments at Gifu University and taught an
intensive summer course as a part-time graduate lecturer
for 10 years.
1.4 IPA/JAXA critical software sympo-
sium
As part of a business project for the Ministry of Econ-
omy, Trade and Industry, I provided guidance on the
implementation of ISO 9000 quality management sys-
tems. In relation to the expansion of ISO 9000 into the
software field, at the request of NTT and Mitsubishi
Electric, I was appointed to the ISO/IEC 15504 Process
Assessment standardization committee. Mr. Tomoyuki
Matsubara, editor of IEEE Software, was a member
of the process improvement committee. He was also
present when I gave my presentation on process assess-
ment at IEEE. Mr. Katahira of JAXA mentioned that
Mr. Matsubara was the chairperson when he first pre-
sented at IEEE. Due to our shared experience as fellow
students, he appointed me as the program chairperson
when JAXA co-hosted the Critical Software Workshop
with IPA.
1.5 Safety Engineering Symposium
I was encouraged to present my findings at the Safety
Engineering Symposium by a former Toshiba employee
from the nuclear power division who had guided me on
safety analysis in the AUTOSAR open-source project.
Between 2006 and 2020, I presented over 20 papers at
safety engineering symposia .[8] [9] [10] [11] [12] [13] [14]
[15] [16] [17] [18] [19] [20] [21] [22] [23] [24] [25] [26][27]
[28]
2 Model
In this section, model means concept models, design
models and operation models on mechanical, electrical,
material and software systems.
2.1 social model
In social models, the opposite is often true depending on
one’s perspective. If you don’t describe the viewpoints
from three or more diﬀerent perspectives, the discussion
can become muddled.
2.2 moter control
The motor design tool JMAGj allows the use of LLM and
MCP through integration with MATLAB and Simulink.
To use LLM with JMAG, it is advisable to add MCP to
JMAG.
3 Process
in this section process means human process and com-
puter process. Automation is the process of replacing
the work of a genius with a computer. Most tasks that
anyone can do have already been replaced by computers.
3.1 wataer fall
In the era when time was stamped on paper cards and
various programs were loaded sequentially into a main-
frame at regular intervals for processing, a person had
to compile the code every few hours. Logical errors or
time stamping errors would waste several hours. It was
necessary to draw diagrams such as flowcharts and input
grammatically correct programs. In two-party transac-
tions, focusing on the aspects where the customer pays
was one way to eﬃcient development. Whether these
customer-funded aspects are called requirements, speci-
fications, or designs depends on the customer’s terminol-
ogy. n mainframes, the CPU, OS, language, database,
and network are pre-configured by the manufacturer,
meaning that half of the specifications are determined
by the computer selection. From an eﬃciency stand-
point, optimizing the work for the aspects the customer
or oneself deems worth investing in can yield reason-
able results. Estimates were based on the assumption
of following the waterfall model, V-model process, etc.,
provided by the computer manufacturer.
3.2 agile
Since the advent of 32-bit CPU PCs, design, build, and
run have become tasks that can be completed by a single
person on a single PC. The order in which these tasks
are performed can be left to the individual’s abilities,
and it has become known that designing in source code
is particularly eﬃcient. Agile is based on almost the
same ideas as those insights gained at that time.
3.3 DEVOPS
LLM has become useful not only for designing and op-
erating systems on the cloud by the same person, but
also for automating collaborative work among multi-
ple people―something that was diﬃcult to achieve with
traditional PCs―from environment setup using Git and
Docker to test operation.
4 services
A service refers to anything where the output can be de-
fined for each input, such as the processing of materials,
the movement of people or materials, or the processing
of information, rather than specifying the exact method
of processing. Another term for this is ”processing in a
dark box.”
4.1 mobility
Mobile machinery includes trains, automobiles, ships,
aircraft, and satellites. The structure of mobile ma-
chinery involves comprehensively designing, prototyp-
ing, and evaluating physical and chemical phenomena,
including the structure, function, performance, materi-
als, fuel, heat, and air resistance of the engine or motor.
4.2 safety system
In situations where humans are outside the hazard
source, such as with manufacturing machinery, the prin-
ciple of isolation is eﬀective. However, in moving objects
where humans are inside the hazard source, the principle
of isolation alone is insuﬃcient. It is crucial to design
for transitions to relatively safer states in all possible
scenarios.
5 tools
Various tools, including CAD, CAM, and CAE, are used
for design, prototyping, and evaluation.
5.1 coding standard
5.1.1 misra C
MISRA C will be restructured to adhere to the spirit
and principles of C, and detailed rules will be rebuilt to
correspond to each applicable version of the C language
standard. Furthermore, the probability calculation of
cases where deviation results in higher quality will be
automated, reducing the unnecessary work of simply ad-
hering to the rules.
5.1.2 CERT C
It automatically generates intrusion, hijacking, and
jamming programs for each corresponding communica-
tion protocol, and uses them to identify vulnerabili-
ties. Based on these results, improvement suggestions
for CERT C/C++ are automatically generated.
5.1.3 STARC RTL design style guide
By creating versions of the STARC RTL Design Style
guide other than Verilog HDL and VHLD, or by auto-
matically converting them to Verilog HDL and VHDL,
we can fill in previously untouched areas.
5.1.4 model based software design
By applying the JMARG guide, we can automatically
generate model inspection tools and create more detailed
guide candidates.
5.2 AI
5.2.1 deep learning
We held a study session on deep learning. A steel com-
pany used a tool that processes multiple models in par-
allel and compares the results to improve the control of
its rolling process.
5.2.2 quantum compuiting
We are considering using LLM to conduct a preliminary
investigation comparing quantum computing algorithms
with conventional optimization techniques in specific do-
mains to determine which approach is more suitable for
which task.
5.2.3 LLM and MCP
By extending MCP (Model context protocol) to other
CAD, CAM, and CAE software, the inter-tool integra-
tion between tools with LLM (Large language model)
capabilities, such as MATLAB, can be dramatically im-
proved.
5.3 UML
In safety-related systems, safety analysis is performed
using state transition diagrams, time series diagrams,
time-series diagrams, and methods such as FTA, FMEA,
and HAZOP.
5.3.1 state machine
There are reports of significantly improved quality com-
pared to conventional methods by automatically gener-
ating Promela code from a state transition diagram to
control a color PS printer, verifying it with SPIN, and
then generating C source code.
5.3.2 sequence diagram
I’m exploring a method that automatically generates
and selects candidate state transitions from a sequence
using LLM, which is the reverse of generating sequences
from state transitions like uppaal.
5.3.3 timing diagram
In a project funded by the Ministry of Economy, Trade
and Industry, we attempted to automatically gener-
ate EtherCAT-compatible control programs from timing
charts. A system could be devised where a mechanical
designer writes control instructions, and the source code
is generated.
6 issue
6.1 Tool Integration
When integrating multiple tools, data and program
transfers may fail due to version diﬀerences. Even with-
out specific errors, the methods for generating and ver-
ifying ways to detect security vulnerabilities and poten-
tial bugs become more sophisticated.
6.2 intellectual property
As patents and copyrighted works increase exponentially
through automated generation, the eﬀort required to
verify who owns the automatically generated intellectual
property will become enormous.
6.3 Responsibility boundaries
Determining the boundaries of responsibility in the
event of an accident, and whether insurance for au-
tomatically generated data is feasible, are social chal-
lenges, just like those for autonomous driving.
7 future work
7.1 formal method
7.1.1 Event B
Bosh was involved in the Event-B project. He once
considered whether automotive software design could
be described using Event-B. The stepwise refinement of
Event-B was a diﬃcult task, requiring only highly skilled
programmers. He wanted to improve eﬃciency by hav-
ing a generative AI generate several candidates.
7.1.2 CSP
The CSP system developed by the recently deceased
Hoare was so complex that only exceptionally skilled
programmers could fully describe it. I want to try to
overcome these traditional diﬃculties with generative
AI.
7.1.3 coq
Microsoft has extended Coq to re-prove the four-color
problem. I would like to explore how LLM can be used
for broader applications of Coq.
7.2 programming language
The goal is to unify the source code of the C and C++
compilers and generate the C and C++ specifications
from the source code. We are also considering extensions
that would allow the use of templates and namespaces
in C.
7.3 operating system
The source code for POSIX PSE51 and OSEK/VDX
OS will be unified, allowing specifications to be gener-
ated from the source code. Ideally, the Priority CEILong
protocol will be introduced to Linux, allowing the selec-
tion of a mode that does not cause deadlocks.
8 conclusion
The extent to which we can entrust generative AI with
harmonizing various perspectives, and what needs to be
checked, is constantly changing.
References
[1] Graduation Thesis: Equivalent exchange research,
Kiyoshi Ogawa, 1982, Hose University.
[2] porting on emulator to Hitachi Computer on PC-
9801, Kiyoshi Ogawa, 1985, Nagoya Institute of
Technology
[3] Graduation Thesis: Pade approximation for simul-
taneous diﬀerential equations, 1986, Nagoya Insti-
tute of Technology
[4] porting VZ editor to N5200, Kiyoshi Ogawa, 1991,
PC-VAN
[5] Testing and Verification for Embedded Linux, Ak-
ihiro Yamana, Kinji watabe, Naoki Saito, Kiyoshi
Ogawa, 2005 in German
[6] 第7 回TOPPERS of the Year 最小セットカーネル
（公募型事業）受賞代表者：斎藤直希、小川清、杉本明加
[7] ETSS を利用した機能安全対応スキル判定と教育訓
練, 小川清, 渡部謹二, 斉藤尚希, 堀武司, 奥田篤, 水口大和, 吉岡律夫, 渡辺登
[8] 安全分析、状態記述と形式手法に着目した安全教育
とスキル堀武司, 小川清, 斉藤直希, 渡部謹二, 森川聡久, 服部博行
[9] 安全関連システムのためのOS の検討, 斉藤直希, 小川清堀武司
[10] 安全に貢献するソフトウェア関連国際規格水野智仁,
森川聡久, 小川清, 斉藤直希, 渡部謹二,, 堀武司
[11] HAZOP 手法の展開, 小川清，斉藤直希，渡部謹二
[12] 自動車制御用プラットフォームの機能安全対応竹内
舞，水野智仁，森川聡久, 小川清，斉藤直希，渡部謹二
[13] 安全関連系の設計のためのHAZOP の展開／小川清，
斉藤直希，渡部謹二
[14] より効率的なHAZOP-TRIZ を利用した設計変更へ
の対応, 小川清, 安全工学シンポジウム, 2014,
[15] HAZOP と関連手法の展開, 小川清, 安全工学シンポ
ジウム, 2013,
[16] ソフトウェアFMEA を体系的に実施する出発点と
してのMISRA-C, 中野泰伸, 原浩晃, 森川聡久, 小川
清, 安全工学シンポジウム2014
[17] 作業診断の国際規格適合とアセッサの訓練, 小川清,
安全工学シンポジウム2014
[18] 安全(safety) と安心(security) に関するC 言語コー
ディング標準の取組安全工学シンポジウム2015 小
川清
[19] HAZOP, FMEA and FTA for Risk Assessment 日本
学術会議安全工学シンポジウムTokyo, July 2, 2015
○小川明秀, 小川清
[20] 安全分析におけるHAZOP-TRIZ 連携の試み小川
清, 安全工学シンポジウム, 2016,
[21] HAZOP-- ‐ TRIZ 連携による交通安全分析, 小川
清, 安全工学シンポジウム, 2017
[22] 機械の制御システムの設計における安全分析の事例
報告尾崎秀典，青島武志，可兒利弘，路海寧，間瀬
剛，松原和音，斉藤直希，小川清
[23] HAZOP とTRIZ を適用した新製品開発とその安全
分析斉藤直希，間瀬剛，松原和音，小川清，寺久保
敏，石津和紀，坪井俊之
[24] 医療システムへのHAZOP 適用松原和音，間瀬剛，
斉藤直希，小川清
[25] 災害支援無線系における安全分析手法の応用小川清，
斉藤直希，間瀬 剛，松原和音，村上 孝，小寺浩
司，福田仁志
[26] 安全分析の図的表現方法、及び設計文書と親和性の
高いツールの提案田中伸明，小川清
[27] 田中伸明
[28] 小川清
[29] 課題に挑む 技術士のソリューション 2009.10-
2012.7, 小川清,
[30] MISRA C bulletin
https://www.misra.org.uk/orum/viewforum.php?f=214&sid=ﬀfdb03a98230bd6e5d3698084a76962
[31] CERT C, Bibliography,
https://wiki.sei.cmu.edu/confluence/display/c/AA.+Bibliography
