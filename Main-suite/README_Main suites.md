**Structure of the suite**: 

**Suites**

The *Main suites* consist of three suites: *Prerequisite (capabilities) suite*, the *Target (capability) suite*, and the *Functional generalisation suite*.

**Sub-suites**

Each suite contains several *Sub-suites*, which in the case of *Target (capability) suite* and the *Functional generalisation suite* represent groups of tasks pertaining to one affordance type and in the case of *Prerequisite (capabilities) suite* specify different types of prerequisite tasks. 

**Experimental paradigm**

Each *Sub-suite* is further divided into various *Experimental paradigms* which test for the same capability but are structured differently, often using different objects or combinations thereof. In the *Target (capability) suite* and the *Functional generalisation suite*, *Experimental paradigms* within a *Sub-suite* that are built around the same core objects have their name start with that object, e.g., Ramp_box, Ramp_box choice or Ramp_distance orientation size. Otherwise, the paradigm name provides a basic description of the paradigm. In the *Prerequisite (capabilities) suite*, however, *Experimental paradigm* names consist of affordance types and objects around which the tasks are built. Not all suites have multiple *Experimental paradigms*.

**Core tasks**

Each *Experimental paradigm* consists of a set of tasks, *Core tasks*, which roughly follow the same basic structure but include some variations (e.g., objects turned differently to create more occlusion) to create differing levels of difficulty within the *Experimental paradigm*. 

**Task variations**

Each *Core task* comes in multiple variations, *Task variations*, following the same structure as the *Core task* whilst varying surface level features such as colour, distance from the goal etc. For each individual task, *Task variations* have been produced through procedural generation. The *Control suites* follow the same structure as described above except for when there is no control task for a given task. 


**Naming convention**: 

Task names were created as follows: Suite_Sub-suite_TaskDescription_TaskVariationHand_TaskComplexity_ForcedChoice_TaskVariationPG.yaml
* **Suite**: A task belongs to either the *Main suites* or the *Control suite*, hence abbreviations ‘Main’ and ‘Control’.
* **Sub-suite**: Each suite contains three sub-suites, the *Prerequisite (capabilities) suite*, the *Target (capability) suite*, and the *Functional generalisation suite*. These are abbreviated as ‘Target’, ‘Prerequisite’ and ‘Generalisation’.
* **TaskDescription**: Refers to the core objects and activities around which each task is built, e.g., FallingWallIllumination.
* **TaskVariationHand**: Certain versions of tasks have been created by hand (as opposed to procedurally generated) because they would be hard to create through procedural generation. Task structure remains the same and the TaskVariationHand hand annotates the feature manipulated. For example, in a given task the gap between two objects is manipulated to create a novel task complexity. Where the gap is small the task would be abbreviated ‘Narrow’ and when it is wide it is abbreviated ‘Wide’. Another example is a task where the reward appears on the left, ‘Left’ or ‘Right’ or else being equal. 
* **TaskDifficulty**: Task difficutly can vary between ‘D1’ (the easiest) and ‘D3’ (the hardest). Task difficulty varies between the *Core tasks* within one *Experimental paradigm* and should not be compared between the *Experimental paradigms*. Note that difficulty estimations are within-task a priori estimates that will not align well across tasks, and might benefit from pos-thoc re-assigning once sufficient populational data is accrued. Task difficulty was approximately determined based on the number of prerequisite capabilities entailed in a task and the number of steps needed to successfully conclude it. When there is only one *Experimental paradigm*, the task automatically gets assigned D1. 
* **ForcedChoice**: This feature gives information about whether a task is structured such that the agent needs to choose between two scenarios or not. Forced choice label can be either ‘FC0’ (not a forced choice structure) and ‘FC1’ (forced choice structure).
* **TaskVariationsPG**: This abbreviation refers to the *Task variations* produced for a given *Core task*. For each newly generated variation, a number is added at the end of the yaml file such as 0001.yaml, 0002.yaml, 0003.yaml. For two features, degree of occlusion and distance from reward, we created labels which will appear at the end of the existent task name. For example, if the reward is far or close from the reward then this will be reflected in the name, 0002_dis_far.yaml and 0003_dis_close.yaml respectively. Labels 'degree of occlusion' and 'distance from reward' were created because they indirectly indicate a degree of task complexity and hence manipulate the degree of capability needed to solve a task. If multiple labels have been created through procedural generation they will be separated by an underscore as follows, 0001_label1_label2.yaml.
  
Example of a task name following the above described convention: Main_Target_BoxChoice_Right_D2_FC0_0003_dis_close.yaml

