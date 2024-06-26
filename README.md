This is a simple windows form C# application i built that allows a user to store their password to specific services in the following format [WEBSITE NAME | USERNAME | PASSWORD] 

STARTUP
when you boot up the program for the first time you will be asked to create a "Master Key" the master key allows you to access your "vault" of passwords, it gets encrypted upon creation
and its very crucial, without it you will not be able to unlock your "vault". the master key gets stored and encrypted in the installation root folder as a file called "PMMASTER.pmd"

when you add passwords to your vault they get encrypted and stored to the root folder aswell in a file called "PMDATA.pmd". these 2 files never get decrypted on the computer itself, they 
only get decrypted in the software. you will notice 2 more files "key.bin" and "iv.bin" these are the "keys" that decrypt your encrypted data. dont delete them as you wont be able to get
back into your current vault as the "PMMASTER.pmd" and "PMDATA.pmd" can only be "unlocked" by the 2 files they were encrypted with (key.bin & iv.bin)
