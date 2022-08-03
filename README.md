# VRCAutolaunch

A lightweight program that Automatically launches external programs with VRChat, 
needs to be run in the background at all times, shows status in the system tray. 

# Usage
To add a program to your Autolaunch, you need to edit the config.json file. <br>
It looks as follows: 
```
{
  "ProgramList": [
    {
      "FileName": "",
      "WorkingDir": "",
      "Arguments": "",
      "StartMinimized": 1,
      "CloseOnQuit": 1,
      "VROnly": 1
    }
  ]
}
```

***"FileName":*** full name of the .exe file <br>
***"WorkingDir":*** is the directory of your executable. <br>
***"Arguments":*** if you need any, can leave empty. <br>
***"StartMinimized":*** determines if the program should be started minimized or normally. <br>
***"CloseOnQuit":*** determines if the program should close whenever the game is closed. Values are either false or true.  <br>
***"VROnly":*** determines if the program should be autostarted only in VR or always. Values are either false or true.

### Example:

```
{
  "ProgramList": [
    {
      "FileName": "ThumbParamsOSC.exe",
      "WorkingDir": "F:/Program Files/ThumbParamsOSC/",
      "Arguments": "",
      "StartMinimized": 0,
      "CloseOnQuit": 1,
      "VROnly": 1
    },
    {
      "FileName": "ThumbParamsOSC.exe",
      "WorkingDir": "F:/Program Files/ThumbParamsOSC/",
      "Arguments": "",
      "StartMinimized": 0,
      "CloseOnQuit": 1,
      "VROnly": 1
    },
    {
      "FileName": "ThumbParamsOSC.exe",
      "WorkingDir": "F:/Program Files/ThumbParamsOSC/",
      "Arguments": "--debug",
      "StartMinimized": 0,
      "CloseOnQuit": 1,
      "VROnly": 1
    }
  ]
}
```
