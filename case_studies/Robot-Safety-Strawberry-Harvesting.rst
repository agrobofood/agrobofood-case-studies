Strawberry harvesting and tending robots
===========================================================
Strawberries are in high demand around the year. To accomodate this demand farmers
are starting to grow strawberries in poly-tunnels, which allow to prolong the harvesting season. 
We also see a trend to growing strawberries in elevated gutter systems and the use of
special strawberry varieties with fruits that grow on long stems an thus hang easily
visible on the side of the elevated gutter. This simplifies harvesting a lot and 
enables automated solutions.


Use case description
--------------------
A strawberry-picking robot is deployed on a strawberry farm. The robot consists of a 
mobile base equipped with a robot arm and an end-effector for picking strawberries. 
The strawberries grow in gutters rows inside a poly-tunnel. The robot moves through 
the rows and picks ripe strawberries that hang down on the sides of the gutters. The 
robot shall be operated in autonomous mode inside the poly-tunnel for harvesting 
strawberries and on the farms premises for travelling to the next poly-tunnel or
to travel to its parking spot.


Related Standards
--------------------

EN ISO 18497: Agricultural machinery and tractors — Safety of highly automated agricultural machines — Principles for design
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
This document gives principles for the design, verification, validation and provision of information for use of 
a highly automated agricultural machine (HAAM). The purpose of this document is to assist in the provision of safety 
requirements, means of verification and information for use to ensure an appropriate level of safety for agricultural 
and forestry tractors and self-propelled machines with functions allowing highly automated operations. It also provides
guidance on the type of information on safe working practices (including information about residual risks) to 
be provided by the manufacturer. This document is not applicable to forestry applications; mobile, semi-mobile or 
stationary machinery used for farm yard or barn operations; and operations on public roads including relevant 
requirements for braking and steering systems. Risks related to the communication between agricultural vehicles
are also out of scope.

**Rational**: The harvesting or tending robot is an agricultural machinery with highly automated operation. It can either
be a tractor (if it also enables towing) or an agricultural machine. This standard only applies to operation in the field.
It seems the standard was also conceived with the open field in  mind. To avoid risks arising from the poly-tunnel environment,
a dedicated risk analysis should be conducted.


EN ISO 4254-1: Agricultural machinery – Safety – Part 1: General requirements
"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
ISO 4254-1:2013 specifies the safety requirements and the means of their verification for the design and construction
of self-propelled ride-on machines, mounted, semi-mounted and trailed machines used in agriculture in order to deal 
with the hazards which are typical for most of the machines. In addition, it specifies the type of information on safe
working practices including information about residual risks to be provided by the manufacturer.

This document deals with significant hazards, hazardous situations and events relevant to this agricultural machinery when
used as intended and under the conditions of misuse foreseeable by the manufacturer during normal operation and service.

ISO 4254-1:2013 is not applicable to

* agricultural or forestry tractors,
* aircraft and air-cushion vehicles used in agriculture,
* lawn and garden equipment,
* machine-specific components or functions (e.g. working tools and/or processes).

ISO 4254-1:2013 is not applicable to hazards related to periodic service, machine conversion and repairs intended to be
carried out by professional service personnel, environmental hazards, road safety (e.g. steering, braking), or to the power 
take-off (PTO) drive shaft; neither is it applicable to guards of moving parts for power transmission except for strength
requirements for guards and barriers.

ISO 4254-1:2013 is not applicable to machines which are manufactured before the date of its publication.

Not all of the hazards dealt with by ISO 4254-1:2013 are necessarily present on a particular machine. A risk assessment
should be carried out by the manufacturer to determine the hazards that are applicable and any hazards in addition to
those dealt with by this part or a relevant machine-specific part. The requirements of a machine-specific part of ISO 4254
take precedence over the requirements of this part.

**Rational**: The harvesting or tending robot can either be just a simple agricultural machine or a tractor. If it can be
classified as agricultural machinery, this standard needs to be applied.


EN ISO 26322-2: Tractors for agriculture and forestry — Safety — Part 2: Narrow-track and small tractors
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
ISO 26322-2:2010 specifies the general safety requirements and their verification for the design and construction of 
narrow-track and small tractors used in agriculture and forestry. It also specifies the type of information on 
safe working practices, including residual risks, to be provided by the manufacturer. It provides technical means 
for improving the level of personal safety of operators and others involved in the course of the normal operation,
maintenance and use of these tractors.
It is applicable to narrow-track tractors having at least two axles for pneumatic-tyred wheels, or having tracks
instead of wheels with a smallest fixed or adjustable track width of not more than 1 150 mm, and to small tractors
having an unladen mass not greater than 600 kg.

**Rational**: The harvesting or tending robot can either be just a simple agricultural machine or a tractor. If it can be
classified as tractor, this standard needs to be applies, as the width of the robot is limited by the width between the 
strawberry gutters. If the robot is classified as tractor and wider than 1.15m part 1 of this standard needs to applied.


EN ISO 3691-4: Industrial trucks — Safety requirements and verification — Part 4: Driverless industrial trucks and their systems
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
This document specifies safety requirements and the means for their verification for driverless industrial trucks
(hereafter referred to as trucks) and their systems. Examples of driverless industrial trucks (trucks of ISO 5053-1)
can also be known as: "automated guided vehicle", "autonomous mobile robot", "bots", "automated guided cart", "tunnel
tugger", "under cart", etc.

This document also contains requirements for driverless industrial trucks which are provided with:

— automatic modes which either require operators' action(s) to initiate or enable such automatic operations;
— the capability to transport one or more riders (which are neither considered as drivers nor as operators);
— additional manual modes which allow operators to operate the truck manually; or
— a maintenance mode which allows manual operation of truck functions for maintenance reasons.

It is not applicable to trucks solely guided by mechanical means (rails, guides, etc.) or to remotely controlled trucks,
which are not considered to be driverless trucks. For the purposes of this document, a driverless industrial truck is a
powered truck, which is designed to operate automatically. A driverless truck system comprises the control system, which
can be part of the truck and/or separate from it, guidance means and power system. Requirements for power sources are not
covered in this document.

The condition of the operating zone has a significant effect on the safe operation of the driverless industrial truck. The
preparations of the operating zone to eliminate the associated hazards are specified in Annex A. This document deals with
all significant hazards, hazardous situations or hazardous events during all phases of the life of the truck (ISO 12100:2010, 5.4),
as listed in Annex B, relevant to the applicable machines when it is used as intended and under conditions of misuse which are
reasonably foreseeable by the manufacturer.

It does not give requirements for additional hazards that can occur:

— during operation in severe conditions (e.g. extreme climates, freezer applications, strong magnetic fields);
— during operation in nuclear environments;
— from trucks intended to operate in public zones (in particular ISO 13482);
— during operation on a public road;
— during operation in potentially explosive environments;
— during operation in military applications;
— during operation with specific hygienic requirements;
— during operation in ionizing radiation environments;
— during the transportation of (a) person(s) other than (the) intended rider(s);
— when handling loads the nature of which can lead to dangerous situations (e.g. molten metals, acids/bases, radiating materials);
— for rider positions with elevation function higher than 1 200 mm from the floor/ground to the platform floor.

This document does not contain safety requirements for trailer(s) being towed behind a truck.
This document does not contain safety requirements for elevated operator trucks.
This document is not applicable to trucks manufactured before the date of its publication.

**Rational**: This standard applies to autonomous mobile robots that are not operated in public zones nor on a public road.
As the robot in the studied use case is only operated on private property this standard can be applied.




Identified standardisation needs
--------------------------------
When looking into this use case a number of standardization needs were identified. As the planned strawberry picking robot classifies
as highly automated agricultural machinery, ISO 18497 was taken as a starting point. The standard is applicable for operation in the
field only and not for operation on the farmyard or in stables. The standard also does not point out whether it can be applied for field
operations in poly-tunnels, which is a different environment than what is encountered in normal fields. The enclosing nature of 
the poly-tunnels takes a number of scape vectors away and adds risks compared to the open field. Therefore, the
robot manufacturer needs to execute an additional risk analysis to identify the risks in a poly-tunnel compared to open fields.
Systems that comply with ISO 18497 need to be equipped with a detection system that is able to detect obstacles 
and persons that approach the robot and the position relative to the robot. When obstacles and persons are inside
warning zone, the robot has to give a warning signal. When the obstacles or persons are inside hazard zone, the robot has 
to enter a safe state. The standard does not give any hints on defining hazard and warning zone around the robot and does 
not reference any relevant standard.
ISO 3691-4 contains detailed information about the design of protective systems for autonomous industrial 
trucks. As the basic concepts of the envisioned mobile robot and industrial trucks is similar, it can be argued, 
that requirements from ISO 3691-4 can be applied to the strawberry picking robot. However, another risk analysis 
needs to support this hypothesis.
Another issue is the autonomous operation on the farmyard. This operation is not covered by ISO 18497. ISO 3691-4 
could be applied if the farmyard is not accessible to the public. Therefore, only a combination of ISO 3691-4 and 
ISO 18497 currently gives sufficient design information to build the strawberry picking robot.
As this example regarding applicability of safety standards to the strawberry picking robot shows even with the 
new ISO 18497 it is still not easy to design a safe autonomous robot that can operate freely on farms. ISO 18497 
is only applicable to operation in fields and not on the farms other premises. Therefore, the robot needs to comply 
with a mixed set of standards (i.e. ISO 18497 and ISO 3691-4). Also 18497 is not very precise when it comes to 
the design of the detection and protection system, which makes it again necessary to base the design on other 
standards and argue their applicability. This case study shows, that there is still a large area of safety for 
autonomous farming robots that is not covered by appropriate standards