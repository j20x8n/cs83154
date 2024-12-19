java c
Utility System   Design 2024–2025
Coursework
Release:                                                                           11/11/2024
Submission:                                                      16/12/2024
Coursework   value:                     30%
IntroductionThe   purpose   of   the   coursework   is   to   provide   you   with   an   opportunity   of demonstrating   the application of knowledge acquired in the course      to a larger scale industrially related   problem. You will make use of knowledge gained in lectures, problem solving, and   computer-based   practicals   (including   available   Guides), and   apply   it   to   produce   a   feasible,   validated   utility   system.
You   have   a   certain   period   of   time   to   produce   the   coursework. You   will   also   be   expected   to apply   your   own   background   skills   as   Chemical   Engineers.You   will   be   expected   to   produce   an   appropriately   structured, written, and   presented   report, with   a   limited   number   of   pages. You   are   provided   with   some   guidance   in   relation to the   structure of the   report to   be   produced,   but   part   of the   assessment   is   to   evaluate   your   skills   in   reporting   the   work   that   you   have   performed, its   validity, and   relevance.The   coursework   is   group   based   –   with   groups   comprising   three   members.   You   are   required to   choose the   members   of the   group   and   register the group   and   members   in   Blackboard.   Marks   are   awarded   for   group   contributions   and   for   individual   contributions.    For   group   contributions,   all   members   of   the   group   are   awarded   the   same   mark.   Individual   contributions   are   to   be   labelled   with   the   member   making   the   contribution.
Overall Requirements
You   are   first   required   to   build   and   simulate   the   existing   operating   conditions   of   a   Utility System, as   illustrated   in   Figure   1, using   the   STAR   v153   software   (group   task).The   second   task   is   to   optimise   the   Utility   System,   with   the   objective   of   minimising   the operating   costs   (group   task). You   are   then   required   to   compare   the   optimal   Utility   System with   the   original   Utility   System.Finally, the   third   task   (individual   task) is   to   modify   and   simulate   the   original   Utility   System (not   the   optimal   Utility   System)   in   order   to   evaluate   improvements   in   heat/power   recovery in   parts   of   the   existing   utility   system   and   so   make   more   effective   use   of   fuel   or   existing equipment.   Each   member   of   the   Group   will   be   required   to   undertake   one   of   the   three modification   tasks   (different   task   each   member). After   you   have   implemented   the   changes,   you   are   required   then   to   compare   these   overall   changes   on   the   utility   system   to   the   original Utility   System.

Figure   1:   Flowsheet   of   the   Utility   System
Legend:
B                              =   Boiler
GT                     = Gas   Turbine
HRSG      =   Heat   Recovery   Steam   Generator
ST                        = Steam   Turbine
L                                 =   Letdown station
P                                 =   Process   (Steam   User)
SG                        = Steam   Generator
De-A               =   Deaerator
Utility   System   DataThere   are   some   missing   flowrate   values   in   the   Utility   System   in   Figure   1 which   you   need to   determine   before   you   start   inputting   the   data   to   STAR.   Site   Configuration   data   should   be   left   as   default   values. Other   relevant   information   is   provided   in   the   tables   below. Current   flowrate data are   required for simulation   purposes while   minimum   and   maximum   flowrate   data   are      needed   for   optimisation   purposes.   Some   values,   for   example   turbomachinery   power, can   only   be   determined   by   the   actual   simulation   of   the   utility   system.
Table 1:   Fuel data
Fuel                                                                                               LHV                                                                        Price
Natural Gas (NG)                                           36,000 kJ Nm–3                                            0.2 $ Nm–3
Fuel Oil                                                                       40,000 kJ kg–1                                                  0.6 $ kg–1
Table   2: Boiler   data
   
Boiler
   
FuelCurrent      Flowrate (kg   s–1)Minimum   Flowrate (kg   s–1)
Maximum
Flowrate
(kg   s–1)
Efficiency
(%)
Blowdown
(%)
Boiler   1
NG
80
0
100
90
2
Boiler   2
NG
90
0
110
85
3
Boiler   3
Fuel   Oil
120
0
120
75
5
Table   3: Gas   Turbine   data
                                                                    Type                                                       Fuel                                            Shaftwork (MW)                                               Casing Losses (%)
GT                            Industrial-based correlation                        NG                                                            110                                                                                            0
Table 4: Heat Recovery Steam Generator data
   
   
FuelCurrent      Flowrate   (kg   s–1)Minimum   Flowrate (kg   s–1)
Maximum
Flowrate
(kg   s–1)
Efficiency
(%)
Blowdown
(%)
HRSG
NG
To   be
determined
Same   as current
Same   as current
73
10
Table 5: Steam Turbine general data
   
ST
Configuration
Shaftwork   model
Isentropic
Efficiency
(%)
Mechanical
Efficiency
(%)
Power
Correction
Factor
ST1
   
GeneratorConstant   isentropic   efficiency
85
   
97
   
1
ST2
85
ST3
80
ST4
75
Table 6: Steam Turbine flowrate data
   
Current   Flowrate
(kg   s–1)
Minimum   Flowrate
(kg   s–1)
Maximum   Flowrate
(kg   s–1)
ST1
Inlet
180
0
200
Outlet   HP
50
0
200
Outlet   MP
130
0
200
ST2
Inlet
100
0
120
Outlet
100
0
120
ST3
Inlet
70
0
100
Outlet   LP
30
0
100
Outlet   Cond
40
0
100


ST4
Inlet
80
0
100
Outlet
80
0
100
General GuidanceIt   is   worthwhile   to   have   looked   at   the   released   Practicals   and   familiarized   yourself with the   STAR   software   before   attempting   this   task.   There      may   be      items      required   that   are not   mentioned   in   the   Guides.   Use   the   Help   system   to   assist   in   these   cases.   As      the      STAR   software      is      frequently      updated, some of the screenshots      may      not   correctly   reflect what you see on   screen.    However, the information you   require for simulation      and optimisation is clearly   provi代 写Utility System Design 2024–2025Matlab
代做程序编程语言ded.Creating   the   initial   model   and   simulation   of   the   Utility   System   can   be   time   consuming. Work   as   a   group   to   discuss   and   overcome   these   obstacles. The   software   will   indicate   frequently,   when   you   select   simulation,   that   values   have   not   been   provided   or there   are   not   enough   degrees   of   freedom   to   perform   the   task.   This   means   that   so   many   values   are   fixed   it   is impossible   for   the   software   to   calculate   appropriate   values   for   those   that   are   missing. Also note   that   you   may   have   too   many   degrees   of   freedom, e.g., there   are   too   many   unknowns and the software cannot   calculate the missing   values.Consequently,   it   is   suggested   that   you   build   up   the   Utility   System   flowsheet   step-by-step,   and   simulate   each   step   before   progressing   to   the   next.    For   example,   input   the   steam headers,   link   them   by   letdown   stations,   add   a   steam   generator   and   then   simulate.   Then add   a   process   load   and   simulate   again.   This   way   it   is   easier   to   resolve   smaller   problems.When   you   have   modelled   and   simulated   the   Utility   System,   you   then   need   to   optimise   it. Within   the   Steam      Network      Environment      in      STAR   there   are   Optimisation   options.   You should    optimise    the      system      by      minimising      the      operating      costs.      When      you      have   simulated   and   optimised   the   original   Utility   System, then   individual   member   tasks   should   be   performed   using   the   original   Utility   System   as   the   starting   point   of   the   modifications.
Individual   Member   1   TaskA senior utility engineer is proposing   to   increase   the   overall   steam   generators’   efficiency.   All   steam   boilers   and   the   HRSG   undergo   a   blowdown   where   heat   (in   the   form   of   saturated   water)   can   be   recovered   to   raise   additional   steam.   Use   this   strategy   to   reduce   the   overall   fuel consumption   by   modifying   the   utility   system.   Model   and   simulate   the   modified   system   and then   compare   with   original   Utility   System   (simulated).
Individual   Member   2   TaskThe   utility   system   manager   is   looking   at   exploiting the   potential   of the   GT/HRSG   system.   There   is   an   opportunity   to   implement   supplementary   firing   and   to   increase   the   temperature of   the   exhaust   gases   entering   the   HRSG   to   850°C,   thus   raising   additional   steam.   Use   this strategy to   reduce the overall fuel consumption   by   modifying   the   utility   system.   Model   and   simulate   the   modified   system   and   then   compare   with   original   Utility   System   (simulated).
Individual   Member   3   TaskPlanned   maintenances   will   reduce   HP   steam   use   by   20%,   MP   steam   use   by   30%   and   LP steam   by   45%.   The   technical   director   of   the   utility   system   believes   that   this   an   excellent opportunity   to   shut   down   the   low-efficient   fuel   oil-fired   boiler,   however   the   load   on   the   NG-   fired   boilers   could   be   increased   if   necessary.   Use   this   strategy   to   reduce   the   overall   fuel consumption by   modifying the   utility system.   Model and simulate the   modified   system   and   then   compare   with   original   Utility   System   (simulated).
Marking   Scheme   and   Report   SubmissionIt   is   up   to   you   to   decide   the   exact   format   of   your   report   and   what   should   be   included   to support   the   work   you   have   done.   A   marking   scheme   and   marking   sheet   will   be   made   available   for      reference      to      help      you      with   this.    However,    the      report      should      include      the following sections:
•          Introduction, Aims   and   Objectives   (Group   - maximum   5 marks)
•          Methodology   (Group   - maximum   5 marks)
•         Original   simulation   results   and   main   features   of   the   utility   system   (Group   -   maximum   30   marks)
•         Optimisation   and   features   of   the   optimised   system   (Group   - maximum   15 marks)
•          Member      1    Task      modification      and      simulation      (Individual      -    maximum      30   marks)
•          Member      2    Task      modification      and      simulation      (Individual      -    maximum      30   marks)
•          Member      3    Task      modification      and      simulation      (Individual      -    maximum      30   marks)
•            Conclusions   (Group   - maximum   5 marks)
Marks   are   also   awarded   for   the   presentation   of   the   report   (Group   - maximum   10 marks).   Total   is   100 marks   maximum   per   group   member.As   the   space   is   limited,   present   the   information   that   you   think   is   relevant   and   reflects   the work that   has   been   done   and the   points that you   are   attempting   to   make   to   an   audience.   Not   all   information   can   be   presented   as   space   is   not   sufficient.   Part   of   the   skill   is   deciding what   is   relevant   and   how   to   express   it.   Do   not   be   verbose.You   will   need   to   include   graphics   from   STAR   (the   simulated   and   optimised   flowsheet). You   may   also   want   to   produce   a   schematic   of   the   type   shown   in   Figure   1. The   most   relevant results   (again   up   to   you   to   decide) should   be   presented   in   your   own   Tables.   These   should include   information   about   the   steam   headers,   fuels,   boilers,   gas   turbines,   heat   recovery   steam   generators, steam   turbines, vents,   letdown   stations, etc.The   report   should   be   completed   in   MS   Word, and   should   not   contain   more   than   24   pages (plus   an   additional   page   for   the   front   cover).   Pages   above   this   limit   will   be   penalized   by   a reduction   of   5% per   additional   page   in   your   overall   mark.Late   submission   of   the   coursework   will   also   result   in   a   penalty   of   a   reduction   in   your   overall mark.   The   later   the   submission   the   larger   the   reduction!   The   reduction   is   set   by the University’s   policy.   If   you   have   any   mitigating      circumstances   that   would   result   in   a      late submission, follow   the   appropriate   policy.   Note   as   this   is   Group   based work   there   are   no   extensions   for   DASS   students.In   addition,   a   pdf   version   of   the   report   should   be   produced   and   it   should   be   uploaded   to   Blackboard.   There   will   be   an   area   in   the   Utility   System   Design   Blackboard   space   for   this and   appropriate   instructions   a week   prior to the   submission date. The   submitted   report   in   Blackboard   will   be   checked   by   TurnitinUK   for   plagiarism   and   collusion.   Be   warned!

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
