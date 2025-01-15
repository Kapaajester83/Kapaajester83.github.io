Navigating Around The OS

Navigating between files, folders, and apps in macOS isn’t particularly tricky, but knowing the right tricks can improve efficiency and make navigation effortless.
Using Finder

https://academy.hackthebox.com/storage/modules/157/1_finder.png

As discussed in the previous section, Finder is the component of macOS that provides the File management functions within the OS. You can use Finder to find and browse files present inside your Mac.
View Root Directory

One way to view the root directory is to launch the Finder app from the Dock, click on the Go Pane at the top, select Computer & click on Storage. 

https://academy.hackthebox.com/storage/modules/157/visit_root_directory.png

Another way to open the root directory is to launch the Finder app from Dock; enter the keyboard shortcut Command + Shift + G, type /, and hit Go. 

https://academy.hackthebox.com/storage/modules/157/visit_root_directory_2.png

You may also go up and down directories in Finder using the Command with the up and down arrows.
Copy and Paste Files & Folders

Just like any other OS, you may copy/paste items in Finder with the right-click menu or the Command + C and Command + V keyboard shortcuts: 

https://academy.hackthebox.com/storage/modules/157/3_finder_pste-2.png

You can also move items by dragging them from one folder to another or even duplicate any item by holding the option key while dragging them.
Cut and Paste (Move) Files & Folders

MacOS does not offer a direct GUI feature to cut and paste files & folders using Finder. But you can use the keyboard shortcut Command + Option + V to move the copied file directly.

    Launch the Finder app from the Dock.
    Right-click on the file or folder you want to move and select Copy.
    Use Finder to head to the location where you want to move a file, and use the keyboard shortcut Command + Option + V to move the file.

Another way to move files in macOS is using the mv command in the terminal, which must be used with caution as it is an irreversible command. To do so, open a terminal from Dock & run the following command to move the Test folder from the Users Document directory into the Users Desktop directory.
Navigating Around The OS

[root@htb]/Users$ mv /Users/htb-student/Documents/Test /Users/htb-student/Desktop/Test

Note: While macOS does not allow "Cut/Paste" of files to avoid potential file loss, it does allow "Cut/Paste" of text through the right-click menu or with the "Command + X" shortcut.
View Hidden Files and Folders

There are lots of hidden files and folders present on macOS that prevent users from accidentally deleting files used by the operating system. However, there are multiple ways to view hidden files on a Mac using the GUI and terminal.

To view hidden files and folders using the GUI:

    Open the folder where you want to see hidden files

https://academy.hackthebox.com/storage/modules/157/org_files.png

Hold down Command + Shift + . (full stop/period)

https://academy.hackthebox.com/storage/modules/157/finder_hidden_files.png

You may also change the default view of Finder to show hidden files, as follows:

    Open a terminal from Dock & run the following commands in Terminal

Navigating Around The OS

[root@htb]/Users$ defaults write com.apple.Finder AppleShowAllFiles true
[root@htb]/Users$ killall Finder

Using Preview Pane

The Preview Pane within Finder allows us to glance at what files and images look like before opening them. It provides instant previews of what’s in each file you highlight with additional information about the file such as Creation Date & Time, Last Modified Date & Time, Last Opened Date & Time, etc.

Enable Preview Pane inside Finder to look at the file preview.

    Launch the Finder app from the Dock.
    Click on the View Pane at the top & select Show Preview. 

https://academy.hackthebox.com/storage/modules/157/Show_Preview-2.png

Now, you can click on any file and see the file's contents on the right side with additional information regarding the file. 

https://academy.hackthebox.com/storage/modules/157/preview_pane-2.png

Finding What You Need

Spotlight is a system-wide desktop search feature of Apple's macOS and iOS operating systems, as discussed in previous sections. Spotlight can help you quickly find items present on your Mac.

Let's try opening a Dictionary in macOS using Spotlight.

    Click on the magnifying glass icon at the top-right corner of the desktop or use the keyboard shortcut (Command + Space bar) to open Spotlight.

Type the keyword dictionary inside the Spotlight search bar and click on the Dictionary app to open a Dictionary instance.

https://academy.hackthebox.com/storage/modules/157/3_spotlight.png

How To Move Around Apps

Moving and switching from one app to another can be tedious, especially if there is a frequent need to split apps every few seconds. To improve efficiency while working on multiple apps, macOS provides features like Mission Control & Split View.
Mission Control

MacOS provides a feature named Mission Control, which offers a bird's-eye view of all open windows, desktop spaces, and apps, making switching between them easy.

There are multiple ways to open the bird's-eye view on your Mac.

    Swipe up using three fingers on your trackpad.

https://academy.hackthebox.com/storage/modules/157/2_mission_control.png

Open the Mission Control app manually from the Launchpad.

https://academy.hackthebox.com/storage/modules/157/1_mission_control_app.png

Split View

By using Split View, you can split your Mac screen between two apps. It would automatically resize the screen without manually moving and resizing windows. Split View only works if you already have two or more apps running in the background.

To use Split View with apps, hover the mouse pointer over the full-screen button (Green Colored) on the top-left, and you will be presented with three options to select from:

    Enter Full Screen
    Tile Window to Left of Screen
    Tile Window to Right of Screen

https://academy.hackthebox.com/storage/modules/157/1_split_view.png

Choose Tile Window to Left of Screen from the menu, and the window will fill that side of the screen. Now hover the mouse pointer onto the next side of the screen and select another app to begin using both apps in split windows side by side.

https://academy.hackthebox.com/storage/modules/157/2_split_view.png

Now that we are system navigation pros, the next section will give us insight into the host's filesystem structure.
Enable step-by-step solutions for all questions
sparkles-icon-decoration
Questions

Answer the question(s) below to complete this Section and earn cubes!
+ 2 Download the above file and double click on it to unzip it. The extracted folder may appear empty, but in reality it has a hidden file with the flag. Can you find the flag?



