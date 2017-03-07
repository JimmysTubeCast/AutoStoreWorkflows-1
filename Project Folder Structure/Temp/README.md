# About The 'Temp' Folder

This folder is used to house local working directories organized for each task inside of the Project folder. As a best practice, the name of the folder inside the **'Temp'** folder should be the same as the **'Task Name'** used.

When Tasks are created in the *AutoStore Process Designer*, a default *Home directory* is automatically assigned, typically with a *GUID* for the sub folder name in the *C:\AutoStore* directory, which lives outside of the Project folder.

Maintaining a Temp folder together with the Project folder is useful in that it prevents the clutter of many additional directories being created, especially for Sales Engineers who frequently find themselves creating many AutoStore workflows.

Also, it aids in troubleshooting issues by being able to go into the Project folder for any jobs which may have been rejected instead of trying to hunt down the automatically generated sub folder, which is usally a named as a GUID.

In certain cases where additional computing power needs to be spread accross larger organizations, a common folder structure for the Project is helpful to maintain consistency accross multiple servers. Jobs can be delivered to other servers by way of Knowledge Package files.

Using a well organized naming convention for Task names is easy to identify, and standardization in naming provides an opportunity for the worklfow creator to simplyfy useful and logical RRT names for dynamic routing within the configuration.


### Capture Tasks
When naming a *Capture* task, it is best to use a lowercase *'c'* at the beginning of the task name, followed by the name of the capture type. 

Examples:
  - cAutoCapture
  - cKonica
  - cKonicaWeb
  - cKyocera
  - cRicoh
  - cRicohWeb
  - cXerox

Within each *Capture* task folder, the following folders should be used for temporary work area sub directories:
  - CaptureHome
  - Rejected
  - TaskHome

> Example:
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\cAutoCapture\CaptureHome
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\cAutoCapture\Rejected
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\cAutoCapture\TaskHome


### Process Tasks
When naming a *Process* task, it is best to use a lowercase *'p'* at the beginning of the task name, followed by the functional name of the task.

Examples:
  - pOCR
  - pBarcodeRead
  - pBarcodeSplit

Within each *Process* task folder, the following folders should be used for temporary work area sub directories:
  - Inbound
  - Rejected
  - TaskHome
  - Working

> Example:
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\pOCR\Inbound
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\pOCR\Rejected
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\pOCR\TaskHome
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\pOCR\Working


### Route Tasks
When naming a *Route* task, it is best to use a lowercase *'r'* at the beginning of the task name, followed by the routing type for the task.

Examples:
  - rToEmail
  - rToFax
  - rToFolder
  - rToSharePoint

Within each *Route* task folder, the following folders should be used for temporary work area sub directories:
  - Inbound
  - Rejected
  - TaskHome
  - Working

> Example:
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\rToEmail\Inbound
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\rToEmail\Rejected
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\rToEmail\TaskHome
> 
> C:\AutoStoreWorkflows\Sample Project\Temp\rToEmail\Working

