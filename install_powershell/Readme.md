##Readme

PowerShell is installed by the Windows Management Framework (WMF). It can be installed as a standalone windows update (.msu).  Normally we'd install this using wusa.exe, but unfortunately it does [not support WinRM](https://support.microsoft.com/en-us/help/2773898/windows-update-standalone-installer-wusa-returns-0x5-error-access-deni). The workaround is to extract the .msu contents and install them using dism.exe.

The folder structure used is as follows:

> **Folder Structure:**

 - PowerShell Version (i.e. **5.1**)
	- OS Version (i.e. **6.3** for Server 2012 R2)
		- Extracted CAB files. These are extracted by using wusa.exe /extract 
	 
