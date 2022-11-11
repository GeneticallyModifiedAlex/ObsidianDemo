# Add a SubModule
#addingSubModule #Git #slides
This allows multliple repo's to be held within a single git repo. The subModules themselves are version controled and can be maintianed.
```
git submodule add https://github.com/GeneticallyModifiedAlex/ObsidianDemo2.git
```
The Project will be added as a folder with the same name as the repo. 

## Cloning a Project with Submodules Empty
#Clone #Git #Submodule
If a parent Repo has submodules within it then cloning has a few additional steps. 
You do however clone the repo as you would any other.
``` bash 
git clone https://github.com/GeneticallyModifiedAlex/ObsidianDemo.git
```
The submodules are added as Empty foldes. To populate the folders you use the following commands.
``` bash
git submodule init
```
This will initialise the submodules Config file.
```bash
git submodule update
```
This will fetch all the data from the project.
There is an [[Git SubModules#]] way to do this that is simpler.

## Cloning a project with SubModules Full
#Clone #Git #Submodule #AlexEdwards
This method will allow you to to have submodules with the relevant content inside using fewer commands. This is done by adding the tag `--recurse-submodules` to the `git clone` command and will automatically initialise and update the submodules in your repository.
```ad-warning
This will cause any submodules that exist within submodules to also be pulled recrsivly. 
This can become a large task if those submodules themselves have submodules.

If you are not sure if this is the case it is safer to use the [[#Cloning a Project with Submodules Empty]] method
```
```bash
git clone --recurse-submodules https://github.com/GeneticallyModifiedAlex/ObsidianDemo.git
```
