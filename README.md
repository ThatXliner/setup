Remember, only install applications to the ~/Application folder

**Before you do anything**: Create a new standard account. This will be the main account. All the steps described below should be ran on the user account. Remember to add the main account to the sudoers file using `visudo`.

## Peripherals
1. Connect a Keychron K3 Pro to the computer
2. Using Bluetooth, connect a Razer Orochi V2 to the computer
3. Disable mouse acceleration and adjust DPI accordingly
	1. either using the native settings (macOS Sonoma+): Settings > Mouse > Advanced > Pointer acceleration
	2. or use LinearMouse
## Native enhancements
1. Menu bar modifications
	1. Show seconds in menu
	2. Show battery percentage in menu bar
	3. Show fast user switching in menu bar![[Pasted image 20240219123319.png]]![[Pasted image 20240219123319.png]]
2. Finder modifications
	1. Modify Finder settings to show path bar
	2. Add Home directory to sidebar
	3. Create an Applications folder in the home directory. Drag apps there, unless specified otherwise
	4. ![[Pasted image 20240219093146.png]]
3. Install Arc: replaces Safari
	1. Set up profiles and sign in accordingly
4. Disable Quick note ![[Pasted image 20240219125234.png]]
5. Install JetBrains Mono, GitHub Monaspace, and MesloLGS NF
6. Install iTerm2: replaces Terminal.app. CLI set up will be covered later
	1. Change the profile by downloading the one from GitHub
	2. Change font. Font size 13
	3. Change theme to minimal![[Pasted image 20240219205146.png]] 
7. Keep the dock icons minimal by only showing apps that are used in this set up process in the dock
8. Install Shottr (from the DMG in the USB): replaces the default screenshot
	1. ![[Pasted image 20240219092909.png]]
9. Install Raycast: replaces default Spotlight
10. Install AlDente: replacing the default battery limiter
	1. Hide Dock Icon
	2. ![[Pasted image 20240219094057.png]]
11. Update hostname (Settings > General > About > Name)
	1. ![[Pasted image 20240219094457.png]]
	2. May need to restart computer in order to take effect
## Creativity
1. Install Final Cut Pro
2. Install Logic Pro with the entire sound library
3. Install MuseScore with MuseHub
	1. Install Muse Keys
	2. Sign in
4. Install Obsidian
5. Install RawTherapee (and drag to system folder)
## Dev tools
1. Install Xcode
	1. Install iOS Sims
2. Install Docker Desktop (and drag to system folder). Set up.
4. Install Postgres. Initialize.
5. Install [GPGTools](https://gpgtools.org/). Import keys
6. On the command line, `xcode-select --install`
7. Setup Git GPG signing
	1. `git config --global commit.gpgsign true`
	2. `git config --global user.signingkey 3E73FE544D567E38` (because that's my signing key)
	3. https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key
8. Setup SSH by copying over the folder from the USB
9. Copy over the projects folder
10. Install VSCode
	1. Install CLI (Search for "shell command")
	2. Setup extensions and themes and keymaps (I didn't back this up 😭)
11. Install Zed (yes, 2 editors)
	1. Sign in
12. Run my dotfiles install script
## Others (Optional)
1. Install UTM
	1. Install a Kali Linux VM
	2. Install a Windows VM
2. Install Minecraft
3. Install Steam
4. Install Roblox
5. Install WPILib
6. Install Discord
7. Install RustDesk
8. Install Notion
