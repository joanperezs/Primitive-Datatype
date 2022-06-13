# Primitive Datatype
### Hecho por Joan Pérez Susidko

## Task 1
Use “Get-Help” to find out more information about 5
cmdlets.
```
Get-Help Get-Help
Get-Help New-Item
Get-Help Get-Alias
Get-Help Get-AuthenticodeSignature
Get-Help Get-ControlPanelItem
```
![image](https://user-images.githubusercontent.com/101748401/173261066-426d4205-3315-4b97-b610-0cd0e4d9c9b2.png)


## Task 2
Use “Get-Help” with the “–Example” parameter for the
5 cmdlets you discovered more about in task 1.
```
Get-Help Get-Help -Examples
Get-Help New-Item -Examples
Get-Help Get-Alias -Examples
Get-Help Get-AuthenticodeSignature -Examples
Get-Help Get-ControlPanelItem -Examples
```
![image](https://user-images.githubusercontent.com/101748401/173261104-464e3372-c4d3-4c1b-aa5c-e9b9917c7346.png)


## Task 3
Create a new text file named “TestFile.txt” under C:\
Maximo\PowerShell\Workshop1\%USERNAME%
```
New-Item -Path C:\ -Name Expo -ItemType Directory
New-Item -Path C:\Sudoblark -Name PowerShell -ItemType Directory
New-Item -Path C:\Sudoblark\PowerShell -Name Workshop1 -ItemType Directory
New-Item -Path C:\Sudoblark\PowerShell\Workshop1 -Name bclark -ItemType Directory
New-Item -Path C:\Sudoblark\PowerShell\Workshop1\bclark\ -Name Testfile.txt -ItemType File
```
![image](https://user-images.githubusercontent.com/101748401/173261292-5d5948e4-a12c-4576-acd1-3b133217fd96.png)


## Task 4
Populate the text file you created in task 3 with all
three datatypes we’ve covered: “Boolean”, “String”
and “Int”
```
Add-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Value True
Add-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Value "Hello"
Add-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Value 42
```
![image](https://user-images.githubusercontent.com/101748401/173261322-6673e7e1-66f6-4a56-b175-7b2197866a86.png)


## Task 5
Read from the text file and use “Get-Member” to find
the datatype returned
```
Get-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt | Get-Member
```
![image](https://user-images.githubusercontent.com/101748401/173261368-7e2d8ead-e0e2-4f22-9b84-f7c74f9a22ba.png)

## Task 6
Overwrite all data within the text file that you created
in task 3.
```
Set-Content -Path C:\Sudoblark\PowerShell\Workshop1\bclark\Testfile.txt -Value "Boooooo"
```
![image](https://user-images.githubusercontent.com/101748401/173261398-4e95f33c-9abe-4076-9546-eafca0562d8e.png)

## Task 7
Format the data returned by a cmdlet into a list
```
Get-Service | Format-List
```
![image](https://user-images.githubusercontent.com/101748401/173261472-b41e94ad-0120-4aa1-9eba-62dba04ddf0f.png)

## Task 8
Pipe “Get-Command” into “Out-GridView”
```
Get-Command | Out-GridView
```
![image](https://user-images.githubusercontent.com/101748401/173261517-a9658314-15a4-4504-b4e2-cb5ea65c91fd.png)

## Task 9
Pipe the 5 cmdlets you discovered in task 1 into “Out-
GridView”
```
Get-Help | Out-GridView
New-Item | Out-GridView
Get-Alias | Out-GridView
Get-AuthenticodeSignature | Out-GridView
Get-ControlPanelItem | Out-GridView
```
![image](https://user-images.githubusercontent.com/101748401/173261555-b2aa2efc-6315-48ca-a860-7058f148d19d.png)


## Task 10
Find the official PowerShell documentation library from Microsoft
![image](https://user-images.githubusercontent.com/101748401/173261698-27d631b4-93ac-48d1-a786-c2f891d16e5f.png)
