# Summary
Brief instructions on installing a custom powershell module.  
<br />

# TL;DR
Download my module files to `<module-directory>\<module-name>\<module-name>.psm1`:
  - Windows PowerShell 5.1: `$HOME\Documents\WindowsPowerShell\Modules\<module-name>\<module-name>.psm1`
  - PowerShell 6/7+: `$HOME\Documents\PowerShell\Modules\<module-name>\<module-name>.psm1`

# Details
PowerShell modules are very powerful and can be quite complex. However most custom PowerShell modules I create simply contain a single standalone function (i.e. cmdlets). As such, to install them, it is sufficient to simply download the relevant module file (PSM1 file), and place it in a subdirectory of your PowerShell profile directory, where the subdirectory is named after the module. This will cause the PowerShell console to automatically load the module when starting, and to auto-load the module when calling it, even if the file wasn't present when starting the console.  

Keep in mind that your profile and module directories have different paths depending on which version of PowerShell you're using. To find out your PowerShell version, enter `$PSVersionTable` at a PowerShell prompt. You can have multiple versions of PowerShell installed (e.g. 5.1 and 7) side-by-side.  

You will need to create these paths if they don't already exist.  
<br />

For my modules:
  - Windows PowerShell 5.1: Download the module file to:
    - `$HOME\Documents\WindowsPowerShell\Modules\<module-name>\<module-name>.psm1`.
  - PowerShell 6/7+: Download the module file to:
    - `$HOME\Documents\PowerShell\Modules\<module-name>\<module-name>.psm1`

:warning: In order for the module to auto-load, it is important that the module file be located in a subdirectory of your modules directory, named after the module itself.  

<!-- Step 1 for "Usage" section of most of my module READMEs:

1. Download `.psm1` to the appropriate subdirectory of your PowerShell [modules directory](https://github.com/engrit-illinois/how-to-install-a-custom-powershell-module).

-->
<br />

For more information about modules see:  
  - Windows PowerShell 5.1: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_modules?view=powershell-5.1#how-to-install-a-module
  - PowerShell 6/7+: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_modules?view=powershell-7.3#how-to-install-a-module
<br />

For more information about profiles, see:  
  - Windows PowerShell 5.1: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-5.1
  - PowerShell 6/7+: https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_profiles?view=powershell-7.3
<br />

For more information about running custom modules as a different user, see: https://github.com/engrit-illinois/how-to-run-custom-powershell-modules-as-another-user.  
<br />

# Notes
- By mseng3. See my other projects here: https://github.com/mmseng/code-compendium.
