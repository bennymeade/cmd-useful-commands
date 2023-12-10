# cmd-useful-commands

## Start TeamCity Agent .bat
```
@echo off
start C:\BuildAgent\bin\agent.bat start
```

## Kill Windows Process .bat
```
@echo off
cd c:\Windows\System32
taskkill /IM CaseHandling.exe /f
taskkill /IM winword.exe /f
taskkill /IM TestDataGeneration.exe /f
taskkill /IM Acrobat.exe /f
taskkill /IM Dw20.exe /f
taskkill /IM OUTLOOK.exe /f
taskkill /IM iexplore.exe /f
```

## Create Folder With Today Date .bat
```
SET TODAY=%DATE:/=-%
SET NOW=%TIME::=-%
XCOPY /S /Y "C:\users\bmeade\Downloads\Test" "C:\Delete\%TODAY%_%NOW%\"
```

## Shutdown PC .bat
```
@ECHO OFF
shutdown -s
```

## Restart PC .bat
```
@ECHO OFF
shutdown /r
```

## Start Caffeine .bat
```
cd C:\caffeine
caffeine.exe 600
exit 0
```

## Run MsTest Via CMD
```
C:\Program Files (x86)\Microsoft Visual Studio 11.0\Common7\IDE>mstest

/testcontainer:D:\TFS\Trunk\Product\Tests\Clipper.AutomationTests\FosAutomation\FosAutomation\bin\Release\FosAutomation.dll

/testsettings:"Trunk/Product/Tests/Clipper.AutomationTests/FosAutomation/local.testsettings" 

/category:batchcase


*** IN FULL

C:\Program Files (x86)\Microsoft Visual Studio 11.0\Common7\IDE>mstest /testcontainer:D:\TFS\Trunk\Product\Tests\Clipper.AutomationTests\FosAutomation\FosAutomation\bin\Release\FosAutomation.dll 
/testsettings:"Trunk/Product/Tests/Clipper.AutomationTests/FosAutomation/local.testsettings" /category:batchcase
```

## XCOPY .bat
```
XCOPY /S /Y "C:\BuildAgent\temp\buildTmp" "C:\Automation Results\ClipperUI.%System.Environment%.%dep.AutomationAcceptanceTests_FosAutomationContinuousIntegration.build.number%.%build.counter%\"
```

## Clear Clipboard .bat
```
echo off | clip
```

## Clear IE cache .bat
```
@echo off
start C:\Windows\System32\rundll32.exe inetCpl.cpl,ClearMyTracksByProcess 255
```
