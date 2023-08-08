# Dual-Boot Lazy Restarter
We want to create a bat to click and automatically restart to other OS.

> How can we do this?
>
> Easy, first we create a .bat file with the next parameters:
>
> ```
> @echo off
> bcdedit /default {}
> shutdown /r /f /t 0
> ```
>
> Now, beetween the brackets **{ }**, we need to type the derised OS **ID**.
> _(just type bcdedit in cmd, loser.)_
>
> ![cmd](https://github.com/gzmatte/Dual-Boot/assets/117684932/5294fd13-f02a-475e-b8aa-50ee51a8fa8c)
>
> Example:
> ![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/6c683cd0-e616-4f0e-ae57-fe4d5aa6b5df)
