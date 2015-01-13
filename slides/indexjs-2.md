## Base Generator functions 1

Inside the 'extend' we have properties called 'actions'.  
Each action can be a function or an object with functions. All the functions inside the object will be executed.  
We have the following actions, in execution order:

* **initializing** - Your initialization methods (checking current project state, getting configs, etc)
* **prompting** - Where you prompt users for options (where you'd call this.prompt())
* **configuring** - Saving configurations and configure the project (creating .editorconfig files and other metadata files)
* **default** - Methods no listed?
