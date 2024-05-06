![image](docs/scoop-logo.jpg)  
###  About [scoop.sh](https://scoop.sh/)
Scoop installs programs you know and love, from the command line with a minimal amount of friction.   


### How install from local manifest?

- Install gradle-8.7
```powershell
scoop install C:\temp\scoop\buckets\gradle\8.7\gradle-8.7.json
```
- Install gradle-8.5
```powershell
scoop install C:\temp\scoop\buckets\gradle\8.5\gradle-8.5.json
```

### How checkout gradle version?

```powershell
scoop which gradle 
# comand output ~\scoop\apps\gradle-8.7\current\bin\gradle.bat
```
```powershell
gradle -v
<# comand output
------------------------------------------------------------
Gradle 8.7
------------------------------------------------------------
#>
```
```powershell
scoop reset gradle-8.5
<# comand output
 Resetting gradle-8.5 (8.5).
 Linking ~\scoop\apps\gradle-8.5\current => ~\scoop\apps\gradle-8.5\8.5
 Creating shim for 'gradle'.
 WARN  Overwriting shim ('gradle.cmd' -> 'gradle.bat') installed from gradle-8.7
 WARN  Overwriting shim ('gradle' -> 'gradle.bat') installed from gradle-8.7
 Persisting .gradle
 #>
```
```powershell
gradle -v
<# comand output
------------------------------------------------------------
Gradle 8.5
------------------------------------------------------------
#>
```