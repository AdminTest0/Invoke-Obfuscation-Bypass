# Invoke-Obfuscation-Bypass


powershell启动Invoke-Obfuscation-Bypass
```
Import-Module .\Invoke-Obfuscation.psd1
Invoke-Obfuscation
```

依次输入选项
```
set scriptpath C:\Users\用户名\Desktop\payload.ps1
token
all
1
out ..\payload1.ps1
```

使用ps2exe将混淆后的ps1文件转为exe
```
.\ps2exe.ps1 -inputFile 'payload1.ps1' -outputFile 'Test.exe' -runtime40 -lcid '' -MTA -noConsole -supportOS
```

![image](https://z3.ax1x.com/2021/08/22/hpTzid.png)
