*This version is updated by Hebah ElGibreen based on [patrolling_sim](https://github.com/gennari/patrolling_sim) to introduce dynamic environment and SAUDE Algorithm (written in the code as ODTA) in addition to ontology with uncertainty.*

This package is to be downloaded on the PC and connected to the [Robot version](https://github.com/hebahG/sim_patrolling_wth_Ontology_Robot) that act as a bridge since the prolog is not compatible with Turtlebot processor (details in **ElGibreen, Hebah, and Kamal Youcef-Toumi. "Dynamic task allocation in an uncertain environment with heterogeneous multi-agents." Autonomous Robots (2019): 1-26.**.

**=======================================================**

**Patrolling Startup Manual**

**=======================================================**

1- on PC setup tcp-interface to have all IP addresses.

2- on PC source and catkin catkin_real_patrolling_semanticN_PCmonitor.

3- on each real robot put catkin_real_patrolling_turtlebot folder.

4- on each real robot put tcp-interface with patrolling-sim (inside src folder).

5- on PC start experement with (niether or virtual option).

6- on real robots start expermintis with it own options.

**=======================================================**

**starting commands for any project**

**=======================================================**
- cd project folder
- catkin_make
- source devel/setup.bash
- catkin_make
- source devel/setup.bash
- cd src/patrolling_sim
- ./start_experiment_distributed.py


_In this version, the start setup was modified to allow starting the monitor, stage, and swi-prolog nodes on a PC instead of robot. Even if there is no virtual robots. This is becuase TK1 processor in robots with armhf OS only use swi-prolog 6.6 which has a connection bug and the newer version is only for x64 and i32 v=OS._

**=======================================================**

**Run Commands On PC**

**=======================================================**
	
	> True on monitor
	> Robot == if want to use virtual robots, then put virtual ==> otherwise put Niether

		
