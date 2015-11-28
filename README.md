# occt.natvis
Customized display of OPEN CASCADE variables content in Visual Studio

Visual Studio provides a way to customize display of variables of different types in debugger windows (Watch, Autos, Locals, etc.).

In Visual Studio 2005-2010 the rules for this display are defined in file autoexp.dat located in subfolder 
Common7\Packages\Debugger of the Visual Studio installation folder (hint: the path to that folder is given 
in the corresponding environment variable, e.g. VS100COMNTOOLS for vc10). This file contains two sections: 
AutoExpand and Visualizer. 

The autoexp.dat or occt.natvis can be added to provide more convenient display of some OCCT data types.

## Usage
1. Download the autoexp.occt and change its name to autoexp.dat, then put it in the folder:%VSINSTALLDIR%\Common7\Packages\Debugger

2. Download the occt.natvis and put it in the %VSINSTALLDIR%\Common7\Packages\Debugger\Visualizers

## References
1. autoexp.dat in %VSINSTALLDIR%\Common7\Packages\Debugger
2. Create custom views of native objects in the debugger. 
   https://msdn.microsoft.com/en-us/library/vstudio/jj620914.aspx 
3. Writing debugger type visualizers for C++ using .natvis files 
   https://code.msdn.microsoft.com/Writing-type-visualizers-2eae77a2#content 
4. stl.natvis in %VSINSTALLDIR%\Common7\Packages\Debugger\Visualizers 
5. qt5.natvis in %VSINSTALLDIR%\Common7\Packages\Debugger\Visualizers
