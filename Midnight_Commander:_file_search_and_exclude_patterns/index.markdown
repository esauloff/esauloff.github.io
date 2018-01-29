Midnight Commander ([site](https://midnight-commander.org/), [wiki](https://en.wikipedia.org/wiki/Midnight_Commander)) is a file manager for *Nix platform.
It is feature-full and supports all basic file and archive operations. And lots more.  

I use Microsoft Windows at my job and there is a great alternative to Midnight Commander -- FAR (File and ARchive) Manager ([site](https://farmanager.com/), [wiki](https://en.wikipedia.org/wiki/Far_Manager)). FAR is powerful as well, it has lots of built-in features and tons of 3rd-party plugins to be added to it.  

But this story is not about FAR at all, it is about some features I miss in MC after working with FAR for 15+ years:
* ability to exclude files or file patterns in search dialog
* shortcut to paste absolute path of currently selected file to console
* MC does not track external changes to directories so it does not auto-refresh directory panels

I spent some time last week to implement first change. It is done for now in my github repository in new branch [feature/exclude-files](https://github.com/esauloff/mc/tree/feature/exclude-files).
As MC Team does not use pull requests, I created internal ticket [#3885](https://midnight-commander.org/ticket/3885) in MC tracking system. Will see where it lands.

Update #1: MC Team replied very quickly with their comments / notes.
Update #2: after MC Team's notes, I did some changes and send everything back. My work is done for now, so will wait if they have some capacity to perform review and their validation in next releases.
