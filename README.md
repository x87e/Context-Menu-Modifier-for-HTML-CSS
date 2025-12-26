# CLI - A collection of useful command line interface scripts

*   Context Menu Modifier for HTML and CSS files.
    - This script adds or removes custom HTML/CSS template links for the
      "New" context menu entry in Windows Explorer.
     
     It works by modifying the following registry values:
     HKEY_CLASSES_ROOT\.html\ShellNew - FileName = "HTMLTemplate.html"
     HKEY_CLASSES_ROOT\.css\ShellNew  - FileName = "CSSTemplate.css"
     
     A base template file for each option is created in this location:
     %%APPDATA%%\Microsoft\Windows\Templates
     You can manually edit these files to customize them as needed.
     
     PLEASE CREATE A RESTORE POINT BEFORE USING THIS SCRIPT!
     It is strongly recommended to back up your system (restore point,
     registry export, or full image) before making any registry changes.
     This takes only a few seconds and can prevent any potential regret.
     
                           For advanced users:
                   ---------------------------------
     - You can open this script in a text editor and modify the registry
       commands or create your own custom versions.
     - If you are unsure about any change, search online for guidance.
     - Editing the Windows Registry (regedit.exe) can cause problems if
       incompatible changes are made, though following instructions usually
       results in only minor registry bloat.
     - This version (v1.0) does not yet support adding fully custom templates.
       That feature will be added in a future update.
