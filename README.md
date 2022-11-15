# Summary
Brief instructions on installing a custom powershell module

# Context
PowerShell modules are very powerful and can be quite complex. However most custom PowerShell modules I (mmseng) create simply contain a single standalone function (i.e. cmdlets). As such, to install them, it is sufficient to simply download the relevant module file (PSM1 file), and place it in a subdirectory of your PowerShell profile directory, where the subdirectory is named after the module. This will cause the PowerShell console to automatically load the module when starting, and to auto-load the module when calling it, even if the file wasn't present when starting the console.  

Keep in mind that your profile and module directories have different paths depending on which version of PowerShell you're using.

For more information about modules see:
  - Windows PowerShell 5.1: 
  - PowerShell 6/7+: 

For more information about profiles, see: 
  - Windows PowerShell 5.1: 
  - PowerShell 6/7+: 

For more information about running custom modules as a different user, see: https://github.com/engrit-illinois/how-to-run-custom-powershell-modules-as-another-user

# Module paths
WIP
