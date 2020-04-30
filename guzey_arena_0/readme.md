Running `guzey_arena_0-plot.ipynb` generates the plot `guzey_arena_0.png`

Running `guzey_arena_0-statistics.ipynb` generates the statistics from the post.

Folder `aimgod_configuration` contains configuration files necessary to replicate the experiment. In order to add guzey_arena_0 to Aimgod, go to your equivalent of C:\Program Files (x86)\Steam\steamapps\common\Aimgod\Aimgod\Custom and copy all folders from the folder `aimgod_configuration` into the selected folder. `aimgod_configuration` contains two folders: `Presets` and `Weapons`. `Presets` contains the file `guzey_arena_0.cust` which will add the guzey_arena_0 scenario to the game and `Weapons` contains the file `SHOTGUN.weap` which will add the Shotgun configuration I used to the game. Make sure to create a copy of the default `SHOTGUN.weap` file.

All other settings I used were default (aside from graphics settings which I set to minimal). I used 2.6.0.3 (early access) version of the game.

Folder `data` contains all data used in `guzey_arena_0-plot.ipynb` and in `guzey_arena_0-statistics.ipynb` in csv format.

Variables **date** and **time** specify the day and the time on which the session was performed. 

Variable **time_in_video** specifies time in each video during which the sample begins.

Variable **condition** specifies whether the sample was taken in control or in treatment (sleep deprivation) condition.

Variable **sleep_deprivation_days** specifies the number of days of sleep deprivation at the time of taking the sample. It is set to 0 for control condition.

Variable **time_elapsed** specifies the time (in seconds) it took to finish the trial. This is the variable on which all statistical analysis is performed.

Folder `graph_archive` contains all major iterations of `guzey_arena_0.png`, preserved for historical interest.

Raw videos that I recorded during the experiment and from which I extracted the data on the round duration are available on [Dropbox](https://www.dropbox.com/sh/y9pt592ghrig4r7/AAAfPxz_l474CMTOkxVn3afLa?dl=0). Note that the video `aimgod-2020-04-16-00-22.m4v` contains 12 samples. I discovered that I miscounted the number of samples I took in that session when I was extracting the data from the video and did not include sample 12 in the data, since the paired sample t-test I use relies on data being matched and my plan was to collect precisely 11 samples in each session.