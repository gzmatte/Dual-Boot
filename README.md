# Lazy Dual-Boot Restarter
### We want to create an icon _(or bat)_ to click and automatically restart to another OS.
---

- First we create a **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/bat.bat)** file with the next parameters:

```
@echo off
bcdedit /default {}
shutdown /r /f /t 0
exit
```

Now, between the brackets **{ }**, we need to type the desired OS **ID**[^1]
[^1]: _(just type bcdedit in cmd)._

![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/04b9a821-99e3-4bb7-9242-3cf1bd5aec9d)

- Done. Save the file & create a shortcut if u want to change the icon. _(Right Click > Properties > Change Icon)_.

</br> 
</br> 

### Now, you can do the same in your other OS. Or automatically set default your primary OS;

- Create this **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/start-bcd.bat)**;
```
@echo off
bcdedit /default {}
exit
```

- Between the brackets type your MAIN OS **ID**. _(or the one you want to keep default)_

- Save and put the bat in _Shell:Startup_
   
```
If u cant open that folder, there's the directory:

"C:\ProgramData\Microsoft\Windows\Start Menu\Programs"
"C:\Users\%USERNAME%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup"
```
Done. After you start the windows, it will set-up default the OS you want.
