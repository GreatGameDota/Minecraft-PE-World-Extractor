# Minecraft Pocket Edition World Extractor

Small repository with files and steps needed to extract worlds saved in Application User Data on Android Devices.

## Steps

- Git clone or download zip of this repo and open the directory

- Connect phone to computer via USB (make sure to have USB debugging enabled (look up how to do that))

- Open command prompt in same directory as this repo

- Run `adb0 devices -l`

- Copy the device serial number

- Run `adb0 -s <copied serial number> backup com.mojang.minecraftpe`

- On phone press "Backup files"

- A `backup.ab` file will now be created in the same directory

- In the command prompt run `abe.jar unpack backup.ab backup.tar`

- A backup.tar file will be created of the backup.ab file
