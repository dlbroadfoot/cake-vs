# Cake for Visual Studio
Adds support for the [Cake](https://cakebuild.net/)
build tool in Visual Studio 2015. Includes support for the Task Runner Explorer, 
new item and project templates and bootstrapping important Cake files

Originally based off Mads Kristensen's [Brunch Task Runner](https://github.com/madskristensen/BrunchTaskRunner) extension.

## Install Cake
In order to use this extension, you must have
[Cake](https://cakebuild.net/) installed on your machine or in your solution.

Use [chocolatey](http://chocolatey.org/) to install it globally by
typing the following in an elevated command prompt:

>choco install -y cake.portable

Alternatively, if you have run the bootstrapper at least once, Visual Studio should automatically discover it (see below).

## Build scripts
The Cake Task Runner automatically triggers when it finds
a `build.cake` file. 

## Task Runner Explorer
Open Task Runner Explorer by right-clicking the Cake script and select **Task Runner Explorer** from
the context menu:

![Open Task Runner Explorer](art/open-trx.png)

Individual tasks will be listed in the task list on the left.

![Task List](art/task-list.png)

Each task can be executed by double-clicking the task.

![Console output](art/console.png)

### Bindings
Task bindings make it possible to associate individual tasks
with Visual Studio events such as _Project Open_ etc.

![Bindings](art/bindings.png)

These bindings are stored in your `cake.config` file.

### Cake installation
The runner will automatically use a project-local copy of Cake if it is already present 
in the current directory or one of the default paths. 
However, at this time, it will not automatically download Cake for you.

## Template Installers
Choose Cake Build from the Build menu to quickly install the default bootstrapper scripts or Cake configuration files into your solution.

![Template installers](art/installers.png)

## Templates

The extension includes an item template for build scripts and project templates for Cake modules, addins, and unit tests.

![Project Template](art/templates.png)

## Contribute
Check out the [Cake contribution guidelines](https://cakebuild.net/docs/contributing/contribution-guidelines)
if you want to contribute to this project.

For cloning and building this project yourself, make sure 
to install the
[Extensibility Tools 2015](https://visualstudiogallery.msdn.microsoft.com/ab39a092-1343-46e2-b0f1-6a3f91155aa6)
extension for Visual Studio which enables some features
used by this project.

## License
[MIT Licence](LICENSE) 
