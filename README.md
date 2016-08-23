# Angular-Tutorial-Heroes-VisualStudio

Angular Tutorial Heroes Using Visual Studio

-Install Node.js® and npm if they are not already on your machine.

Verify that you are running node version 4.4.x - 5.x.x, and npm 3.x.x by running node -v and npm -v in a terminal/console window. Older versions produce errors.

-Set up Visual Studio for TypeScript

Ensure you have the latest version of Visual Studio 2015 installed. Then open Visual Studio and install the latest set of TypeScript tools as follows:

Open Tools | Extensions and Updates.
Select Online in the tree on the left.
Search for TypeScript using the search box in the upper right.
Select the most current available TypeScript version.
Download and install the package.

-Create the Visual Studio ASP.NET project

-Copy the QuickStart files into the ASP.NET project folder

-Restore the required packages

Right-click on the package.json file in Solution Explorer and select Restore Packages. 
This uses npm to install all of the packages defined in the package.json file. It may take some time.
If desired, open the Output window (View | Output) to watch the npm commands execute.
Ignore the warnings.
When the restore is finished, a message should say: npm command completed with exit code 0.
Click the Refresh icon in Solution Explorer.
Do not include the node_modules folder in the project. Let it be a hidden project project folder.

An error such as "@angular/compiler is not in the npm registry" suggests that Visual Studio 2015 is using an older version of npm. Update to the latest installed version of npm:

Tools | Options to open the Options dialog.
In the tree on the left, select Projects and Solutions | External Web Tools.
On the right, move the $(PATH) entry above the $(DevEnvDir) entries. This tells Visual Studio to use the external tools (such as npm) found in your path before using its own version of the external tools.
Click OK to close the dialog.
Restart Visual Studio for this change to take effect.

-Edit the TypeScript configuration file

For Visual Studio 2015 we must add "compileOnSave": true to the TypeScript 

-Build and run the app

Compiler errors such as "Property ‘map’ does not exist on type ‘Observable’" and "Observable cannot be found" indicate an old release of Visual Studio. 
