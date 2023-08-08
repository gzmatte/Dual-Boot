# Dual-Boot Lazy Restarter
We want to create an icon to click and automatically restart to another OS.

> First we create a **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/bat.bat)** file with the next parameters:
>
> ```
> @echo off
> bcdedit /default {}
> shutdown /r /f /t 0
> exit
> ```
>
> Now, between the brackets **{ }**, we need to type the desired OS **ID**.
> _(just type bcdedit in cmd)._
> 
> ![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/04b9a821-99e3-4bb7-9242-3cf1bd5aec9d)
>
> Done. Save the file and create a shortcut if u want to change the icon. _(Right Click > Properties > Change Icon)_.


Now, you can do the same in the another OS. Or create a startup file to automatically set default your primary os.
> Create this **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/start-bcd.bat);
> ```
> @echo off
> bcdedit /default {}
> exit
> ```
> Between the brackets type your MAIN OS **ID**. (or the one you want to keep default)
> Save and put the bat in _Shell:Startup_
