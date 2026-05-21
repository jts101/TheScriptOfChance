# TheScriptOfChance (Versions 1-3) Remastered

# WARNING!

I am NOT responsible for ANY damages done to your computer! Note that running the destructive parameters of the script MAY result in a broken Windows installation! The script does **NOT** delete any personal files, however it could damage system files and cause the system to stop booting into Windows completely. I recommend ONLY running the destructive parameters in a virtual environment, or on a spare system you don't care about whatsoever!

This PowerShell script runs a random command each time you execute the script! It can also run programs or open websites! Most commands are good, however some can be bad (depending on the parameter used). It's a command roulette script, anything can happen!
Feel free to record and react to the script (if you wish), as the script does some very unexpected things that would for sure cause you to have a great reaction!

# Some notes before running:
- The script works the best on Windows 10 and higher. I have not tested older Windows 10 versions, but I think they will work too. TSOC has **a LOT** of logging, and Windows 7 will **NOT** run the script due to it. Windows 8.1 will, however it might spit it out in the PS window itself. I might make a script in the future for Windows 7 and 8.1 if there's enough demand for it.
- The parameters are **NOT** case sensitive, meaning it won't matter if you type ``-SafeMode`` or ``-safemode`` for example.

# TheScriptOfChance Versions:
- There are 3 scripts, TheScriptOfChance 1.0, TheScriptOfChance 2.0, and TheScriptOfChance 3.0. TSOC 2 & 3 has lots of new commands in it, but some of the older ones were either reworked or removed. Some commands however are the same. TSOC 1.0 used to have 3 separate scripts, however I decided to restructure the script and add parameters, as it's more efficient that way.

# TheScriptOfChance 1.0 Parameters:
Note: Without a parameter runs with ``-ND`` (Non destructive).
- ``-ND``: Non destructive, safe to run on main! (However could BSOD or reboot but should recover).
- ``-NDnr``: Non destructive, however it won't reboot or BSOD!
- ``-NDna``: Non destructive, however does not open random apps (Since there's a lot in this script!)
- ``-SD``: Semi Destructive, may damage your system! (Have a system restore point or VM snapshot!)
- ``-SDna``: Semi Destructive, however no random apps!
- ``-FD``: Fully Destructive, may NOT be able to recover and may need to reinstall Windows or restore VM snapshot!
- ``-FDna``: Fully Destructive, however no random apps!

# TheScriptOfChance 2 & 3 Parameters:
Note: Without a parameter runs with ``-SafeMode``.
- ``-SafeMode``: Only safe commands are ran, safe to run on main, no commands will disrupt your work!
- ``-Unsafe``: Runs commands that could potentially be unsafe only! Note not every command is unsafe, but could be unwanted.
- ``-SemiUnsafe``: Combines SafeMode and Unsafe parameters, no Deathwish commands!
- ``-VeryUnsafe``: Runs commands that could potentially be unsafe, plus DeathWish commands (Very bad!)
- ``-DeathWish``: Bye bye Windows Installation (high chance!)
- ``-All``: Every command in this script is an option, Run with caution!


# Before running the script:
- Be sure to run ``Set-ExecutionPolicy Bypass -Force`` before the script (You only need to do this ONCE!) If you want to set the ExecutionPolicy for this PowerShell session only, you can run this command instead: ``Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process -Force`` **NOTE:** You would have to re run this if you closed the PS window! You could alternatively run the script with this instead (If you want it to bypass each time you run it): ``powershell -ExecutionPolicy Bypass -File .\TSOC-3.ps1 -SafeMode``. Just provide the script name and parameter, and make sure your PowerShell window is in the SAME directory as the script! I gave an example for TSOC 3 safe mode, but you can change it to any of the parameters you wish!). 
- If you did set the execution policy, then you type in ``.\TSOC-1.ps1``, ``.\TSOC-2.ps1``, or ``.\TSOC-3.ps1`` (along with a parameter, example: ``.\TSOC-3.ps1 -SafeMode``) and press enter to run. After that, you can press up arrow again to be able to pull up the same command to run it again (You can also do that with the other command if you did not set the policy).
- For best results, put the script in the C drive to easily access it, then do ``cd \`` to go to the root of the C drive, then run the command! I always do this in virtual machines as it's faster.
- For better results, run PowerShell as TrustedInstaller if running the destructive parameters (Winaero can do it under "Run as TrustedInstaller" or you can use AdvancedRun, which is what I use instead since I don't need to install another program for it). Note that some commands do not like being ran as TI and may fail.
- NOTE: The script logs to the location of C:\Logs. These logs will say the commands that were executed, so you can check it later to see what it did! There may be additional logs in there, as some commands do create other logs. Some logs may also go to the desktop and/or temp folders on the system. More about the logs below.
- Another note: some commands **may** take longer to execute, so if it's blinking, give it time! I tried to fix this with the "Loading, please wait.." messages. Also be sure you didn't accidentally select in the PowerShell window, as that pauses it! If you did, right click anywhere in the window and it should unpause!
- If you have any questions, feel free to ask me! I am glad to answer any questions! If you have any command suggestions, tell me them as I could implement them into TSOC 2 & 3!

# The logging system:
As you know, it logs to C:\Logs, however here's what each log is used for:
- TSOC_3_Log: This is the PowerShell transcript. It logs everything about the PS session and what runs. It's a bit longer.
- TSOC_3_CMDLog: This logs the commands that were executed, and only the commands!
- TSOC_3: Some of the scripts in TSOC itself have their own logs, they get dumped in here.

Depending on what version of TSOC you run, the number may differ in the log name.
### NOTE: TSOC 1 will have similar logs, however some may be different compared to TSOC 2 & 3. Also, TSOC 1 is no longer being updated, and will continue to stay the same. TSOC 2 and 3 however will continue to get updates, check back here for them!

Also, 
# PLEASE DO NOT RUN THE DESTRUCTIVE VERSIONS ON YOUR MAIN, IT CAN BE DESTUCTIVE!
- If you want to run them, MAKE A SYSTEM RESTORE POINT! It can recover most damages, however I would avoid DeathWish, as that may require a FULL Windows reinstall (Depending on the command that was executed).

Anyways hope you enjoy using my script! It took a long time to develop (as I've been working on TSOC since early 2024).
Also thanks to the help of Gemini and ChatGPT for some commands ideas, as well as other people I know! I did write some of these myself, however.
