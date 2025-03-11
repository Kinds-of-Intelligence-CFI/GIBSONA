# GIBSONA
Gibsona is a novel battery for the assessment of affordances in artificial agents. It contains templates for generating config files for Animal AI environments that test an agent's ability to assess the affordances of objects in the environment and the generalisation of the agent to new distributions in the environment.

Exisiting configs can be found in Variations.zip. If you want to generate your own config files you first need to install the Animal AI procedural generation tool.

Once that is installed run the following commands:
```
procgen sample-bulk -o ./Variations/Control-suite 'Control-suite\' 100
procgen sample-bulk -o ./Variations/Main-suite 'Main-suite\' 100
```bash 

You will then have a folder Variations that contains 100 configs for each of the different templates in the Control-suite and Main-suite. You can also set a seed for the random generation using the option -s <seed>.
