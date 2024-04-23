**Structure of the suite**: 

The *Main suites* consist of three suites: the *Prerequisite (capabilities) suite*, the *Target (capability) suite*, and the *Functional generalisation suite*. 

Each suite contains several Sub-suites, which in the case of *Target (capability) suite* and the *Functional generalisation suite* represent groups of tasks pertaining to one affordance type and in the case of *Prerequisite (capabilities) suite* specify different types of prerequisite tasks. 

Each sub-suite is further divided into various *Object types*. In the *Target (capability) suite* and the *Functional generalization suite*, this classification specifies the object used in *Experimental paradigms*. In the *Prerequisite (capabilities) suite*, however, *Object types* classification refers both to the objects and affordance types. 

Each *Experimental paradigm* consists of a set of tasks, *Basic tasks*, that test for the same capability but are structured differently, often using different objects or combinations thereof. Not all suites have multiple *Experimental paradigms*. 

Each *Basic task* comes in multiple variations, *Task variations*, following the same structure as the main task whilst varying surface level features such as colour, distance from the goal etc. 

**Naming convention**: 

Task names were created as follows: Suite_Sub-suite_TaskDescription_TaskVariationHand_TaskComplexity_ForcedChoice_TaskVariationPG.yaml
* **Suite**: A task belongs to either the Main suite or the Control suite, hence abbreviations ‘Main’ and ‘Control’.
* **Sub-suite**: Each suite contains three sub-suites, the *Prerequisite (capabilities) suite*, the *Target (capability) suite*, and the *Functional generalisation suite*. These are abbreviated as ‘Target’, ‘Prerequisite’ and ‘Generalisation’.
* **TaskDescription**: Refers to the core objects and activities around which each task is built, e.g., FallingWallIllumination.
* **TaskVariationHand**: Certain versions of tasks have been created by hand (as opposed to procedurally generated) because they would be hard to create through procedural generation. Task structure remains the same and the TaskVariationHand hand annotates the feature manipulated. For example, in a given task the gap between two objects is manipulated to create a novel task complexity. Where the gap is small the task would be abbreviated ‘Narrow’ and when it is wide it is abbreviated ‘Wide’. Another example is a task where the reward appears on the left, ‘Left’ or ‘Right’ or else being equal. 
* **TaskComplexity**: Complexity can vary between ‘C1’ (the easiest) and ‘C4’ (the hardest). Task complexity varies between *Basic tasks* within one *Experimental paradigm* and should not be compared between the Experimental paradigms. Task complexity was not formally determined but is rather an approximate determination based on how many prerequisite capabilities are entailed in one task and how many steps need to be taken to successfully conclude a given task. When there is only one *Experimental paradigm*, the task automatically gets assigned C1. 
* **ForcedChoice**: This feature gives information about whether a task is structured such that the agent needs to choose between two scenarios or not. Forced choice label can be either ‘FC0’ (not a forced choice structure) and ‘FC1’ (forced choice structure).
* **TaskVariationsPG**: This abbreviation refers to the *Task variations* produced for a given *Basic task*. For each newly generated variation, a number is added at the end of the yaml file such as 0001.yaml, 0002.yaml, 0003.yaml. For two features, degree of occlusion and distance from reward, we created labels which will appear at the end of the existent task name. For example, if the reward is far or close from the reward then this will be reflected in the name, 0002_dis_far.yaml and 0003_dis_close.yaml respectively. Labels 'degree of occlusion' and 'distance from reward' were created because they indirectly indicate a degree of task complexity and hence manipulate the degree of capability needed to solve a task. If multiple labels have been created through procedural generation they will be separated by an underscore as follows, 0001_label1_label2.yaml.
  
Example of a task name following the above described convention: Main_Target_BoxChoice_Right_C2_FC0_0003_dis_close.yaml

