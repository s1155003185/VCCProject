# VCCProject
Versioning-Coding-Corporation Project

## History

As I am handling large Document Project, find that current document processor does not support versioning.
Also, existing document processors have some interesting behaviour, such as
- When save, will save from beginning.
- Auto create new style.
- When press Enter at Title, the new line will have new style that make the content disappear.
- When having outline then save, document cannot save correctly.
- The Index cannot recognize item number. When save, item numbers disappear.
- When handling thousand pages document, it lags. Some will hang and quit. 
- Docx cannot save as docx by default.
- Cannot save in local storage by default.
- Security Problem.
etc.

As those have not be solved till now, I believe that they are properties instead of bugs. I better to write a document processor myself.
When I try to write a document processor with versioning, I find that I should write a git application instead of document processor. But I need to write a document processor before creating a git application project. As most codes are mechanical work, I write a code generator to write those projects instead of writing one by one. So, I need to write 3 applications.

Firstly, I try to use SwiftUI + dynamic library first as I don’t need to create website and handle payment progess but I can find no way to create virtual ListView.
Secondly, as SwiftUI seems difficult to me, I try to use C# + dynamic library as I am experienced in C#. But I found that Linux and MacOS does not support C# and Visual Studio does not support multi-platform, then I give up.
Thirdly, I try to use Java + dynamic library as Java is multiplatform. But I find that NetBeans has not supported C++ long time ago.
Fourthly, I try to use VSCode with g++. Then I try about one month to setup the makefile. In fact, there are no templates for multiplatform with gtest. I need to study and write makefiles (both library and executable) from the beginning.
In fact, I am experienced in coding among 10 years, but I still used about 6 months to start a project. Beginner should use more than one year. To write an engine, it might use more than 6 months.  I think I better write a program to skip one year effort.

## Members

VCC Project Members include the followings:
Status: 
-	Pending: Coming soon
-	Active: Keep implementing, will change without notification.
-	Stable: Workable.
-	Inactive: Will not update in future.

### FastStartup

#### SimpleTemple (libSample) (Free) [Waiting to finalize]

Simple Template for multiplatform dynamic library. 
Free to change and use in any purpose.

#### SimpleTemple (Sample) (Free) [Waiting to finalize]

Simple Template for multiplatform executable. 
Free to change and use in any purpose.

#### VCCModule (libVCCCore + Java/SwiftUI/Other UI) (Free) [Active]

Project Template that easy to use and update. No need to create project from the beginning every time.
If want to update code, just drop the External/vcc folder then download the new one.
VCCModule  is a package of Static components of  ProjectStarter with following components:
Core:
-	Helper
-	Macro
-	Exception
-	Log Service
-	Action Manager
-	Etc.
Module:
-	TextEditor
-	Document
-	Speedsheet
Free to change and use in any purpose.

#### VCCProjectGenerator (Free) [Pending]

Generate VCC standard dynamic library project with VCCModule.
After setup Enum, then can generate dynamic library automatically.
Free to use in any purpose.

#### FastStartup (SubScription) [Pending]

Based on VCM module (View-Control-Model) to generate multiplatform UI + dynamic library project.
After designing structure of application (UI Design), then can auto generate code project. What remains are handling custom logic.
Do not need any configuration, can update code project directly.
UI => API => Action => Model => API => UI

### ProjectHandler (Free/SubScription)

Git Application with following features:
-	Normal Git Operation (Free)
-	Git for Document / Spreadsheet Versioning (Subscription)
-	Git for Project Inheritance (Subscription) (Note: Too many versions for VCC Project.)

### VCCOffice (Free/Subscription)

Office with Document, Spreadsheet, Notepad with versioning
