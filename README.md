##Prepare a New Script File

This small script was simply made to make the creation and editing of scripts easier. The general usage is like this:

`prepfile [FileName] [-e EditorToUse]`

Basically, feed the script the name of the file you want to make/edit, and if you want, give it an editor to use. If you do not give it an editor to use, it will use the default one that is set in the script (which can be changed easily).

When you run the script, it will make a file if it does not exist (the file does not need to be in the current directory) and open it in the chosen editor. At this point you can then write the script and save the file. To continue with the script close the editor (this is not needed in some editors) and the script will ask if you want to give it some arguments to pass. The script will then be run and the output displayed to the terminal like normal. Once the script ends, it will look at the exit code and determine if it failed or not. If it did fail it will then ask if you want to edit the script some more and restart the process.

 I tried to make it as modular as I could so that it can be expanded on easily. This way it can be easily customized to fit whatever kind of situation that you have. The exit codes can be changed to whatever works best for the system, and the command for the editors are run directly, meaning that you can add arguments to it if you would like.
