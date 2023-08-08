# Dual-Boot Lazy Restarter
We want to create a icon to click and automatically restart to another OS.

> First we create a .bat file with the next parameters:
>
> ```
> @echo off
> bcdedit /default {}
> shutdown /r /f /t 0
> exit
> ```
>
> Now, beetween the brackets **{ }**, we need to type the derised OS **ID**.
> _(just type bcdedit in cmd)._
>
> _like this;_
> 
> ![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/04b9a821-99e3-4bb7-9242-3cf1bd5aec9d)
>
> Now,
