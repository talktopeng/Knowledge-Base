# Installation



# How to install oh-my-posh
https://www.hanselman.com/blog/my-ultimate-powershell-prompt-with-oh-my-posh-and-the-windows-terminal
https://ohmyposh.dev/docs/installation/windows

Open a PowerShell prompt and run the following command:
<pre>winget install JanDeDobbeleer.OhMyPosh -s winget</pre>
Upgrade 
<pre>winget upgrade JanDeDobbeleer.OhMyPosh -s winget</pre>
# Fonts
**oh-my-posh font install**
<pre>> oh-my-posh font install</pre>


Once you have installed a Nerd Font, you will need to configure the Windows Terminal to use it. 
This can be easily done by modifying the Windows Terminal settings (default shortcut: CTRL + SHIFT + ,). 
In your settings.json file, add the font.face attribute under the defaults attribute in profiles:
<pre>{
    "profiles":
    {
        "defaults":
        {
            "font":
            {
                "face": "MesloLGM Nerd Font"
            }
        }
    }
}
</pre>

In vscode terminal or Windows terminal, run <pre>code $profile</pre> to get your currenn environment profile.  
Put this line your profile.

<pre>oh-my-posh --init --shell pwsh --config ~/jandedobbeleer.omp.json | Invoke-Expression</pre>
or <pre>oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH\jandedobbeleer.omp.json"</pre>

In vscode, CTRL + , to open settings
<pre>{
    "workbench.iconTheme": "material-icon-theme",
    "files.exclude": {
        "**/.git": false
    },
    "security.workspace.trust.untrustedFiles": "open",
    "files.autoSave": "afterDelay",
    "editor.fontFamily": "Cascadia Code",
    "terminal.integrated.fontFamily": "MesloLGS Nerd Font"
}</pre>
