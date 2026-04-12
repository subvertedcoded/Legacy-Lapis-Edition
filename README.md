# Current Progress
~~0, none, nada. I'm still figuring out how to start :(~~

Was able to build the fpkg and run it on my slim 12.00. This is a good place to start :)

Please also note, at this time this is practically just the base unmodifed jp version of LCE at least at the writing of this readme. I'll probably look at hooking up the networking stuff revelations has or something

# Info
~~No idea if any of this will be possible. I do not know jackshit about the OpenOrbis toolchain, the normal sony sdk for that matter, and I'm still very clueless regarding what I should look at for getting this to work as a PS4 homebrew app, but hopefully it'll work out :)~~

After some tinkering, successfully building a fpkg, and properly installing and running said fpkg onto my 12.00 PS4, I think I can confidentally say that this project is possible with the files we have. Originally, I was planning on migrating to the OpenOrbis toolchain if neccissary, however aside from slightly tinkering with the provided param.sfo and creating a gp4 file for the file structure, the codebase is probably capable of being used as a base for porting features such as direct connect to servers to LCE dedicated servers and maybe future releases. 

# Original Codebase Info

At least from what I was able to gather from files such as the param.sfo, the original codebase was made for the jp release of LCE for version 1.00 (not 100% sure if it was actually 1.00). Some information seemed a bit off, such as the content id in the param.sfo file stating JP0127-CUSA00283_00-MINECRAFTPS00000 when it should be JP0127-CUSA00283_00-MINECRAFTPS40000. 

# How can I build and Run this???
I will not be providing fpkgss in the repository, and so you will be required to manually build the fpkg yourself after cloneing the source code.

1. Go to the homepage of the repository and click the big green button named "Code". Click download zip from the submenu that pops up and extract and place it into a folder of your choosing. 

2. Go to the [CyB1k's Fake PKG tools](https://github.com/CyB1K/PS4-Fake-PKG-Tools-3.87/releases) repository to the release section and download and place the .rar file into another folder seperate from the one in step 1. For reference, I'm using the latest version of making of this readme which is 7.00.

3. In the fpkg tools, open gengp4_app.exe, select the ./Minecraft.Client/PS4_Game directory and generate and save the GP4 file.

4. Close the gp4 creation tool and open the orbis-pub-gen.exe tool. Click file, open, and select the gp4 file from step 3 (or the premade one in ./Minecraft.Client/PS4_Game directory). Click the build button, select the location, and let it build.

5. Take your newly created fpkg and install it onto your homebrewd PS4. The game requires a minimum firmware of 4.50.


# Contact
Uhhhh I mean feel free to ping me in the [LCE hub discord server](https://discord.gg/eemHDKS78n) I guess. My username is realsubvert.  
