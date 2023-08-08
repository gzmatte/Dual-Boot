# Dual-Boot Lazy Restarter
We want to create a bat to click and automatically restart to other OS.

> First we create a .bat file with the next parameters:
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
> _like this;_
>         ![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/6c683cd0-e616-4f0e-ae57-fe4d5aa6b5df)
