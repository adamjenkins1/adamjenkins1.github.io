---
layout: default
title: projects
group: "navigation"
---

<h2>Most Notable Projects</h2>     
<ul>
<h3 style="display:inline;">Custom Linux File Server</h3>
<h4 style="display:inline; float:right;">January - March 2017</h4>
<p>
This server was built to aid Terra Nova High School Journalism easily backup their 
files essential to printing the Terra Nova Times newspaper. While getting an AWS server, 
or additional space on Google Drive for file storage would have been ideal, 
there simply wasn't a budget for it, which is why I decided to build something myself. 
In order to ensure reliability and ease of use, I decided to create a custom version of Ubuntu 
that had OpenSSH already installed, and install that version of Ubuntu on a 1 TB external hard 
drive. This would allow anyone with that hard drive to start the server from a live boot, 
which means that the server could be started using any computer, and that necessary files 
would only be stored on that external hard drive. If you are not familiar with the idea of 
live booting, basically what it means is that you create a temporary session of Ubuntu by 
booting from this hard drive and selecting "Try Ubuntu without installing." In this mode, 
the drivers are generalized, so it is possible to live boot from nearly any working computer. 
The only problem is that this session is temporary, so anything not included in the base install 
will be erased on reboot. To solve this problem, I created a separate NTFS partition 
on the external hard drive so data saved in this partition will persist after reboots. 
I also wrote a Python script to be run once Ubuntu had successfully started that will 
test the network connection, mount the NTFS partition, start OpenSSH, and display to the 
user the port OpenSSH is running on, and the server IP address. At this point, the user 
can go to any computer on the same network, connect using an SFTP client, and backup or 
copy any files they choose.  Multiple users may also connect and access the sever at the same
time. Due to the security risks and time it would take to implement properly, 
I chose not to forward any ports on the server, so it is only available locally.
</p>

<h3 style="display:inline;">Python File Backup Script</h3>
<h4 style="display:inline; float:right;">January - March 2017</h4>
<p>
I'm a tad bit paranoid about losing files, so generally what I used to do to backup everything
I cared about locally was to put it into a gzipped tarball (similar to a zip file) and 
then upload it to a Linux server.
This became tiresome after a while, so I decided to write a Python script to automate
the process.  The script takes the host and the user name as command line arguments. 
Once started, it will call a bash alias I called "archive" to throw all necessary files 
into a gzipped tarball and name it according to the date.  This step is skipped if the 
archive already exists. Next, using a SSH library called Paramiko, the script 
connects to the given server, deletes the old archive (it would be best to save them to 
keep a record, but space can be an issue) if it exists, and begins uploading the new archive. 
Once the new archive has successfully been uploaded, the script will exit.  The script is run
like this: <code>./backup.py --host HOSTNAME --user USER NAME</code>, but that became 
a lot to type all the time, so I wrote additional bash aliases to make it a bit easier. 
Now all I have to do now to backup my files is type <code>backup-[SERVER_NAME]</code>, 
and the script is called with the correct command line arguments. I have access to three 
different Linux servers, so all I have to do to backup to all of them is 
type <code>backup-all</code>, and the script is run for each server.
</p>

<h3 style="display:inline;">TN Rotational Schedule</h3>
<h4 style="display:inline; float:right;">January - August 2016</h4>
<p>After being pitched the idea, I created the TN Rotational Schedule mobile app 
for Terra Nova High School, located in <a href="https://www.google.com/maps/place/Terra+Nova+High+School/@37.6802822,-122.4596628,11z/data=!4m5!3m4!1s0x808f709c80d33127:0x118d2aa0ddff4e4b!8m2!3d37.5946419!4d-122.4761369" target="_blank"> Pacifica, CA</a>. TN Rotational Schedule is now availble on the <a href="https://itunes.apple.com/us/app/tn-rotational-schedule/id1135302983?ls=1&mt=8" target="_blank">App Store</a> and <a href="https://play.google.com/store/apps/details?id=com.adam.rotationalschedule&hl=en" target="_blank">Google Play</a>, 
free of charge.  The app is designed to aid students, parents, and staff by providing an accurate and 
reliable source of information about the rotational schedule and class times. The code for both the 
<a href="http://github.com/adamjenkins1/ios-Rotational-Schedule-app" target="_blank">iOS</a> and 
<a href="http://github.com/adamjenkins1/Rotational-Schedule-App">Android</a> versions can be found on Github.</p>

<h3 style="display:inline;">BBLeagues Basketball Database Project</h3>
<h4 style="display:inline; float:right;">String 2016</h4>
<p>I completed this database in Spring 2016 while taking the databases course, CINS 370. 
BBLeagues was built using Oracle and contains a variety basketball related statistics. 
In order to better understand the data, we created our own .csv files from the data using PL/SQL, 
usually containing one or two statistics, and plotted said .csv files using R. After taking our 
findings to our professor, we were asked to present to the class. The presentation I built using LaTeX 
and presented can be found <a href="Data/media/pdf/main.pdf" target="_blank">here</a>.</p>
</ul>
