# <p align="center">🌹❤Fix❤🌹</p>

## **1. Download GeForce Experience [v3.20.3.63](https://fichiers.touslesdrivers.com/64580/GeForce_Experience_v3.20.3.63.exe)**
Uninstall current GFExperience app from control panel. Not the drivers, just the Experience app

Sign in into GFE with nvidia account. Its recomeneded to create a temp mail account as it will later not be needed for anything.
<p align="center">
  <img src="https://github.com/Shhezita/FIX/assets/32721494/43a13c81-9904-4594-aa71-446961266be3" />
</p>

## **2a. Auto Install [FIX](https://github.com/Shhezita/FIX/releases/download/1.2/AutoInstall.ps1) and [app.js](https://github.com/Shhezita/FIX/releases/download/1.2/app.js)**
**Download and extract release, right-click  AutoInstall.ps1 and choose Run as Administrator**
You may need to allow the script to run on your system. 

To do this run powershell as administrator, then run this powershell call :

   ``` Set-ExecutionPolicy RemoteSigned```
  
   ``` Set-ExecutionPolicy Unrestricted```

Type "A" then hit enter and re-run AutoInstall.ps1

## **2b. Manual Install [app.js](https://github.com/Shhezita/FIX/releases/download/1.2/app.js)**
Fully close GFE, if needed use task manager.
Download, and replace the default app.js with the one downloaded. 

app.js location:
 ```
 C:\Program Files\NVIDIA Corporation\NVIDIA GeForce Experience\www
```
<sup> App.js changes explained [HERE](Manual.md) <sup>





## **3. Hosts**    

Open hosts file in a text editor (notepad++)  

    C:\Windows\System32\drivers\etc\hosts 
    
  > *(copy-paste the file on your desktop to edit, copy back to "etc" folder if you have permission errors)*


**Add at the end of the file :**

    127.0.0.1 international-gfe.download.nvidia.com
    127.0.0.1 gfwsl.geforce.com
    
**Or just download and drag [hosts](https://github.com/Shhezita/FIX/releases/download/1.2/hosts) if you dont have any more blocklists**
## **4. CMD**
Open cmd and enter to apply hosts

    ipconfig /flushdns

<p align="center">
  <img src="https://github.com/Shhezita/FIX/assets/32721494/6c44e290-27ea-437d-9d16-7e3178391c0f" />

</p>

## **5. GFE**
> Start GeForce Experience and in settings enable in game overlay, as shown
<p align="center">

  <img src="https://github.com/Shhezita/FIX/assets/32721494/68b754f7-96a1-4836-bf80-a752c00dc9c0" />
</p>
