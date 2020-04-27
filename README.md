# ThemeKit

![banner](https://github.com/MTACS/ThemeKit/blob/master/images/banner.png)

## A unified macOS theming platform

[Installation and creating themes](https://github.com/MTACS/ThemeKit/wiki)

###

[Download](https://github.com/MTACS/ThemeKit/releases/download/v1.0/ThemeKit.zip)

### 

Sample theme layout

```└  Satine.bundle```
   
      └ Info.plist
   
      └ com.apple.AddressBook
       
      └ com.apple.AppStore
    
      └ com.apple.FaceTime
    
      └ com.apple.finder
    
      └ com.apple.iChat
   
      └ com.apple.mail
    
      └ com.apple.Music
    
      └ com.apple.Preview
    
      └ com.apple.systempreferences
    
      └ com.brave.Browser
    
      └ com.microsoft.VSCode
    
      └ com.tinyspeck.slackmacgap
   
      └ com.apple.Terminal

We suggest having all Apple icons themed when using a theme, this is because the previews are loaded from a selected theme, true icon randomization will come later.

###

ThemeKit requires SIP (System Integrity Protection) to be disabled to theme icons. This is because in newest macOS versions, certain files cannot be modified. ThemeKit uses methods built into AppKit to change icons. Removing a theme resets icons to stock macOS. 

On macOS Catalina, new methods prevented ThemeKit from working properly with just SIP disabled. This is because a new read only partition was added to Catalina called /System which cannot be modified. This requires us to remount it as read write, something similar to jailbreaking on iOS. This can be done by running ```sudo remount -uw /``` followed by your password. This is only temporary as it will be reset to read write upon boot, so this command can be run only when you need to change a theme after reboot. 

Any system apps, as well as user apps installed via a .pkg usually have read/write permissions disabled. In order for ThemeKit to apply icons this must be set to enabled. Once a theme has been applied, it can be disabled again, although will require these steps to be repeated when changing, applying or removing a theme. 

###

ThemeKit is considered an experiment, and is provided as is. This does not rely on code injection, and requires certain security measures to be disabled, albeit temporarily. 

##

Icons in screenshots are [Glacier](https://glaciericons.com/) with some of my own icons in that style. Banner space image found [here](https://www.spacetelescope.org/images/heic1105a/)

