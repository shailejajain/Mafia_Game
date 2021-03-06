Online Mafia: A new take on the classic game of murder!
Created by Zach Belateche, Carlos Guanche, Shelley Jain, & Isabelle Wolff

To use the standard server, ec2-52-8-76-50.us-west-1.compute.amazonaws.com,
simply download and extract the game files. Next, run the client as follows:
    1. In command line, navigate to the folder "game-master"
    2. Run the command "java Client" to run the client
    
To use a third party server, edit line 27 of the client class to contain
the IP or DNS of your desired server (still port 10101). Then recompile the client:
    1. In command line, navigate to the folder "game-master"
    2. Run the command "javac Client.java"
Now run the client the same way you did before.

The game uses standard rules for the most part. However, there are a few changes:

Characters:
Of course there is the traditional, mafia, doctor, detective, and villagers but we’ve added a new character called The Poltergeist and modified the way the mafia are selected.
The sneaky little Poltergeist chooses a citizen, whose vote will be randomized when voting for the mafia, so instead of submitting a vote for who they actually consider is the mafia, the chosen ones’ vote will be randomly generated by the computer.
Based on the number of people playing, we choose one mafia for about every 4 people playing the game. The first mafia is randomly chosen by the computer. However, in the beginning of the game, the administrator has the option to allow the computer to randomly choose the remaining mafia or to allow the first mafia to recruit the remaining mafia until the preset limit of mafia is reached. If the admin chooses our version, each night until the maximum capacity of mafia is reached, the first mafia will be able to recruit any live citizen to join its crew and that citizen has the option to join the mafia or remain whatever character it initially holds.
The Will:             
Any character can now enter a will at any time during the game, as long as he or she is still alive. Once that character dies, their will will be displayed to the world. 