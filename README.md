# Lazy Dual-Boot Restarter
> We want to create an icon _(or bat)_ to click and automatically restart to another OS.


- First we create a **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/bat.bat)** file with the next parameters:

```
@echo off
bcdedit /default {}
shutdown /r /f /t 0
exit
```

- Now, between the brackets **{ }**, we need to type the desired OS **ID**. [^1]
[^1]: **(just type bcdedit in cmd).**

![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/04b9a821-99e3-4bb7-9242-3cf1bd5aec9d)

- Done, Save & create a shortcut if u want to change the icon. [^2]
[^2]: **(Right Click the Shortcut > Properties > Change Icon).**

-----

### Now, you can do the same in your other OS. Or automatically set default your primary OS;

- Create this **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/start-bcd.bat)**;
```
@echo off
bcdedit /default {}
exit
```

- Between the brackets type your MAIN OS **ID**. [^1] _(or the one you want to keep default)_

- Save and put the bat in Shell:Startup. [^3]

[^3]: **If u cant open that folder, go to "C:\ProgramData\Microsoft\Windows\Start Menu\Programs"**

### Done. After you start the OS, it will set-up default the OS you selected.




</br> 
</br> 
</br> 
</br> 
</br> 
</br> 
</br>
