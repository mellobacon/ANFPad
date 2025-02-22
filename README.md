<h1 align="center" style="position: relative;">
    <a href="https://github.com/ANF-Studios/ANFPad"><img width="200" style="border-radius: 50%;"
            src="./src/images/display.png" /></a><br>
    ANFPad
</h1>

<h3 align="center">ANFPad, a small project by ANF-Studios<br>A simple application that manages all your notes</h3>

<p align="center">
    <a href="https://github.com/ANF-Studios/ANFPad/blob/master/LICENSE">License</a> •
    <a href="https://discord.gg/fKWpK7A">Discord Server</a> •
    <a href="https://github.com/ANF-Studios/ANFPad/releases/latest">Download</a> •
    <a href="https://github.com/ANF-Studios/ANFPad/blob/master/CHANGELOG.MD">Changelog</a>
</p>

<h2 align="center">Using it</h2>
<p>You can grab the latest release of <a href="https://github.com/ANF-Studios/ANFPad">ANFPad</a> at the <a
        href="https://github.com/ANF-Studios/ANFPad/releases/latest">releases</a> section and run the installer like any
    other Electron application.<br /><strong>Note:</strong> At the moment, the GUI version is only a pre-release, so you
    would have to use that if you feel eager for it.</p>

<h3>I'm living on the Edge, give me the latest features</h3>
<p>You can simply grab a pre-release with the latest features or works that are under development. Keep in mind that
    things may break or appear unexpectedly.</p>

<h3>I want to compile my own version</h3>
<p>Well, you're in luck, there are two ways instructed in this file:</p>
<h4><strong>[RECOMMENED]</strong> Using PowerShell</h4>
<p>Prerequisites:
    <a href="https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell">PowerShell</a>, <a
        href="https://git-scm.com/downloads">Git</a> and <a href="https://nodejs.org/en/download/">NodeJS</a>.
    Now save the following code in a <code>ps1</code> (such as <code>run_anfpad.ps1</code>) file and run it with
    PowerShell.
</p>

```ps1
$desktop = [Environment]::GetFolderPath("Desktop");
cd $desktop;
[Console]::Write("[GIT] Cloning respository...\n");
git clone https://github.com/ANF/ANFPad.git $desktop\ANFPad;
[Console]::Write("[NPM] Installing node_modules...\n");
npm install;
# Start ANFPad
[Console]::Write("[ELECTRONJS] Building ANFPad...\n");
npm run start;
[Console]::Write("[NPM] Starting...\n");
# Uncomment this part if you want an installer file.
# [Console]::Write("[ELECTRONJS] Creating installer...\n");
# npm run publish;
# [Console]::Write("[NPM] Created installer...");
# cd out\make\squirrel.windows\ia32;
# Invoke-Item .
```

<h4>Doing it manually</h4>
<ol>
    <li>Download the repo:</li>
    <a href="https://github.com/ANF/ANFPad/archive/master.zip"><img
            src="https://user-images.githubusercontent.com/68814933/103164783-7a4ad080-47dd-11eb-8796-bc45d5019b4f.png"
            alt="Download the repo"></img></a>
    <li>Extract the (downloaded) zip file.</li>
    <li>Open up a terminal such as command prompt.</li>
    <li><code>cd</code> into the directory you downloaded.</li>
    <li>Run <code>npm install && npm run start</code></li>
</ol>

<h2 align="center">Further help</h2>
<p>You can <a href="https://github.com/ANF-Studios/ListManager/issues">create an issue</a> or just join the support
    server.</p>

<a href="https://discord.gg/fKWpK7A"><img
        src="https://discord.com/api/guilds/732064655396044840/embed.png?style=banner3"
        alt="Chat in the server"></img></a>
