<div align="center">

## IP Algoritme


</div>

### Description

This code can calculate the decimal number of an IP-Adres. You can use the number everywhere like http(s),ftp,proxy(s),and other! So if you don't want to give people an IP-Adres, just give them the decimal number!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[MijoSoft](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mijosoft.md)
**Level**          |Advanced
**User Rating**    |3.2 (19 globes from 6 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Encryption](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/encryption__1-48.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mijosoft-ip-algoritme__1-66516/archive/master.zip)





### Source Code

```
Function IP_Nummer(ip As String) As String
Dim nrs() As String
If Len(Replace(ip, ".", "")) = (Len(ip) - 3) Then
nrs = Split(ip, ".")
If nrs(0) >= 256 Or nrs(1) >= 256 Or nrs(2) >= 256 Or nrs(3) >= 256 Then
MsgBox "The IP-Adres is invalid!", vbCritical + vbOKOnly, "Error!"
Exit Function
End If
a = nrs(0) * 256
a = a * 256
a = a * 256
b = nrs(1) * 256
b = b * 256
c = nrs(2) * 256
d = nrs(3)
nummer = (a) + (b) + (c) + (d)
IP_Nummer = nummer
Else
MsgBox "The IP-Adres is invalid!", vbCritical + vbOKOnly, "Error!"
End If
End Function
```

