# Dual-Boot Restarter
> This is only a read-me file.
----------------------------

We want to create an executable batch to click in there and automatically open the other OS.

How can we do this?

Easy, first we create a .bat file with the next commands:

```
@echo off
bcdedit /default {}
shutdown /r /f /t 0
```

Now, beetween the brackets {}, we need to type the other OS ID.
(just type _bcdedit_ in cmd _loser_)

![Screenshot](https://github.com/gzmatte/Dual-Boot/assets/117684932/b4b5725b-a523-4f90-b696-d752a2775bf7)
.
![Example](https://github.com/gzmatte/Dual-Boot/assets/117684932/6c683cd0-e616-4f0e-ae57-fe4d5aa6b5df)
