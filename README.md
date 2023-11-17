## Lazy Dual-Boot
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

- Done. 

> Create a shortcut if u want to change the icon. [^2]
[^2]: **(Right Click the Shortcut > Properties > Change Icon).**

![Screenshot_8](https://github.com/gzmatte/Dual-Boot/assets/117684932/fdca03b2-2ea5-44d6-8585-cb9f32bb9459)

### Now, you can do the same in your other OS.

-----

You can set the default primary OS automatically with this; 

- Create this **[.bat](https://github.com/gzmatte/Dual-Boot/releases/download/1/start-bcd.bat)**;
```
@echo off
bcdedit /default {}
exit
```
- Between the brackets type your MAIN OS **ID**. [^1] _(or the one you want to keep default)_

- Save and put the bat in Shell:Startup.
> (U can put this in the secondary so after a restart you go back to the main OS)

### Ready!

</br>

</br>

</br>

</br>

</br>

</br>


