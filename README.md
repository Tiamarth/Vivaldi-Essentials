# Vivaldi Essentials 

Vivaldi Essentials is a group of css files that add various features or enhancements to Vivaldi's interface. The main css was originally a part of my Vivaldi skin, [AFV](https://github.com/Tiamarth/Arc-for-Vivaldi), but I became of the opinion that they were outside the necessary scope of the skin and decided to move them to their own project. The other css files are random bits of code I wrote either on the forums or on the Vivaldi subreddit to answer other peoples' requests for custom mods or solve other peoples' issues with the interface. I believe all of these changes should be in Vivaldi by default, available as settings to tweak.

## Features:

`ve_main.css`  
- add a 1px window border that persists when native window is disabled  
- reduce amounts of empty, unused space in various places  
- hide Vivaldi's built-in titlebar when GUI is hidden  
- when tabs are not at the top of the window, merge address bar with header  
- Remove Vivaldi's ugly header gradient  

`ve_autohideAddressbar.css`  
- autohide addressbar  
**Note:** do not use `ve_autohide_Addressbar.css` if your address bar is at the bottom. It will not work as intended.

`ve_operaPanel.css`  
- make the panel appear to merge with the Vivaldi menu icon, similar to Opera's panel  

`ve_mergeTabsAddress.css`  
- merge the address bar with the tab bar  
**Note:** do not use `ve_mergeTabsAddress.css` with `ve_autohideAddressbar.css`. It will not work as intended. Also, don't use it if your tabs aren't at the top of your browser. `ve_mergeTabsAddress.css` will break if your window gets too small. If your resolution is smaller than mine you may need to adjust the values in the css. Honestly, given all the special circumstances for this particular feature, I may remove it until I can do it with javascript.


## Installation

First, find `style` in your Vivaldi install directory. It should be in the following places depending on your platform:

**Linux:** `/opt/vivaldi/resources/vivaldi/style`  
**Windows:** `%localappdata%\Vivaldi\Application\[version]\resources\vivaldi\style`  
**Mac:** `/Applications/Vivaldi.app/Contents/Versions/[version]/Vivaldi Framework.framework/Resources/vivaldi/style`

Now, download the css files corresponding to the features you want, and drag them into that folder.

Then open `resources/vivaldi/browser.html` in a text and add the following to `<head>`  
`<link rel="stylesheet" href="style/[css_file_name_here]" />`

For example, if you only wanted to use the main features of this mod, you'd add the following to the head: `<link rel="stylesheet" href="style/ve_main.css" />`

If you want to use multiple files, just repeat the above for each one. You need to add a line for every file you want to use.

**Need more help?** Get in touch!
- add me on Discord: Tiamarth#6729
- join my [Discord server](https://discord.gg/ZfDP2ZV)
- [Create an issue here on GitHub](https://github.com/Tiamarth/Arc-for-Vivaldi/issues/new)
- [Email me](mailto:tiabusy@gmail.com)

Don't email me unless the other methods fail for some reason. Email is not a great way to contact me.
