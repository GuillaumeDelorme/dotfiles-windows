# Dotfiles and things to do after fresh Windows install

## Install usefull apps

Install winget-cli : https://docs.microsoft.com/en-us/windows/package-manager/winget/#install-winget

Execute this PowerShell script :
```ps1
$packages = @(
    '7zip.7zip'
    'BlenderFoundation.Blender'
    'GIMP.GIMP'
    'Git.Git'
    'Inkscape.Inkscape'
    'Microsoft.WindowsTerminal'
    'OpenJS.NodeJSLTS'
    'Rustlang.rust-msvc-x64'
    'Ytmdesktop.Ytmdesktop'
)

foreach ( $package in $packages ) {
    winget install --id=$package -e -h
}
```
