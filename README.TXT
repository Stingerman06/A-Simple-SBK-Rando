What this is:

A simple Snowboard Kids randomizer for the N64 that randomizes a ROM you already own.


What this isn't:

A randomized Snowboard Kids N64 ROM generator.



Pre-requisites

1. Make sure you're using the version "Snowboard Kids (USA).z64"
2. If your ROM isn't a .z64, you can convert it from .n64/.v64 using the N64 byteswap program, Tool64. The .z64 is Big Endian, so use that option.
3. Make sure your ROM is CLEAN. This program will reject any changes make to your ROM previously, so if it isn't clean, you'll know it.
4. Make sure you have the rn64crc tool also downloaded, as you will need to correct your ROM's CRC when randomizing your game.
5. An N64 Emulator of your choice(I personally recommend Project64).


How to use:

1. Open up "Simple Randomizer Maker.exe"
2. Select your ROM/game with the .z64 extension
3. Select any options you'd like to use
4. Select any number of seeds(number of randomized games)
5. Tick on/off Generate Spoil Log if you want to spoil yourself of anything(not really helpful with this build of the randomizer)
6. Click Randomize
7. Use the rn64crc tool to correct the CRC(so your game can boot up in the emulator. instructions below)
8. Enjoy!


How to use the rn64crc tool if you don't know how...

1. Before loading your game, open up your command prompt/powershell, since this program uses console commands to use
2. Place your newly randomized game in the same folder as rn64crc.exe
3. Change the command window's current directory to the directory rn64crc.exe is in.

Example:

	cd "C:\Documents\rn64crc"

4. Since I have to give permissions to the program to run, I have to add .\ to the beginning of mine, but run it with -h for all possible commands like so.

Example(my written use. The '.\' is a permission I have to grant in the window):
	
	.\rn64crc.exe -h

5. Write that but with -u instead of -h and it updates the CRC if the CRC is incorrect.


After the CRC is corrected, the game is ready to play!



Things to note!

This particular randomizer is far from perfect, and not even close to cleaned up in it's current state. The randomizer
uses a Python script pre-built engine with some options, but it's far from flexible. There's no if-type command
flexibility, thus balancing things around and having more control over specific things is really difficult using this.

That said, do keep in mind this program can fail to generate a successful seed at times, but I can't seem to pin-point
why. It's hard to decipher since the only debugging this program has isn't the best or easiest when it comes to
debugging. Example being, there's no debugging when a seed fails to generate, thus I cannot figure out what went wrong
in the randomization process.

In short, if the seed doesn't generate, just make another one.


This will be made public 'as-is' and this particular randomizer will never be updated. This was a learning experience
for me and the only things I learned was Python Code is quite buggy from the first iteration I made, and making a
randomizer can be simple if you know what you want to change around.



Links to related programs used/required:

Simple Randomizer Maker(used to make this):
https://github.com/Mips96/SimpleRandomizerMaker

Real N64 CRC Tool(required):
https://www.smwcentral.net/?p=section&a=details&id=8799


If the links are broken, or if something is just flat out broken(which will definitely happen), drop it in "Issues".


Randomizer by Stingerman06
