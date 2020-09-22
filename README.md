<div align="center">

## The Windows98 code converted to VB


</div>

### Description

This is the VB version of the Windows98 code
 
### More Info
 
heh, read the title


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Brandon Burr](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/brandon-burr.md)
**Level**          |Unknown
**User Rating**    |4.8 (43 globes from 9 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Jokes/ Humor](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/jokes-humor__1-40.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/brandon-burr-the-windows98-code-converted-to-vb__1-3731/archive/master.zip)





### Source Code

```
Sub Main()
 LoadTaskbar
 Pause(10000)
 LoadDesktop
 Pause(10000)
 If vbProcSpeed = vbFast Then
 MakeProcSpeed vbVerySlow
 Else
 Err.Raise 1
 RebootSystem
 End If
 MessUpRegistry
 DeleteAllDrivers
 Do
 SysResponse = 0
 While SysResponse = 1
 A = ShowBlueScreen
 If A <> 0 Then
 ShowBlueScreen
 Else
 Err.Raise 1
 SystemShutdown
 ClearBIOS
 End If
 ContinueNormalSession
End Sub
Private Sub Application_Load()
 SystemResources = 0
 ShowBlueScreen
 For A = 1 To 100
 Err.Raise 1
 Next A
 ActiveApp.Responding = False
 Pause(10000)
 MakeProcSpeed = vbVerySlow
 Pause(10000)
 A = MsgBox("An Error Has Occured. Reboot system?",vbYesOnly,"Duh")
 If A = vbYes Then
 MsgBox "Error: Unable to reboot system. Too useless."
 Err.Raise 1
 Else
 MsgBox "Too Bad!"
 Err.Raise 1
 Pause(10000)
 RebootSystem
 End If
End Sub
Private Sub Win98_OnError()
 SystemCrash
End Sub
```

