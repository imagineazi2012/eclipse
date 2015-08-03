# eclipse
eclipse jre or jdk missing. I had eclipse installed on my laptop which i have used severally to run java programming but but suddenly displayed this ugly face erorr. This I fixed manually by adding some parameters in the eclipse initialization file, saved and ran it. And wow! error flag disappeaared. 
if you have similar issue like mine, please feel free and try my solution.
if you are running the 32bit version then this should work
open your eclipse.ini file, highlight everything, delete, copy this one below, paste and save then run your eclipse

-showsplash
org.eclipse.platform
--launcher.XXMaxPermSize
256M
--launcher.defaultAction
openFile
-vm
C:\Program Files (x86)\Java\jre1.8.0_45\bin\javaw.exe
-vmargs
-Dosgi.requiredJavaVersion=1.5
-Xms40m
-Xmx512m    

But if you are using 64bit version then removing the (x86) from the above path should get you running too.
