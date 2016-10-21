# How to get up and running with MRC CLIMB

### Accessing your machine

This section assumes that you have your <ip_address> and <password> from your local CLIMB super user. You can access your machine in a variety of ways, the main two of which are detailed below. 

**Galaxy** – if you aren’t comfortable with the command line, **try this option first!**.
1. In a modern web browser (i.e. not Internet Explorer) navigate to <ip_address>/galaxy
2. Register for an account within Galaxy by going to 'User' in the top menu bar. Make a note of your username and password. This will allow you to save your progress between sessions. If you don't register an account, your work will be deleted within a day or two.
2. There are loads of galaxy tutorials available from [the galaxy project wiki], as well as the [ABPRI] website, which is aimed at microbial genomics.

**ssh on windows** - if you are comfortable with the command line and have a windows computer
1. Install [putty] followed by [mputty], you then have to point mputty to the putty.exe file via the 'Tools' menu of mputty. (This is because mputty is a wrapper for putty, so it needs putty installed as well, and it needs to know how to find it).
2. In the 'Server' menu, go to 'Server name', put in your <ip_address>, put 'ubuntu' as your username and enter your password, then press 'OK'.
3. Your <ip_address> should show up on the right hand side, double click on it. It will open a new tab in mputty, although you may need to put your password in again. You have to type it in, copy and paste does not seem to work.

**ssh on mac** - if you are comfortable on the command line and have an Apple computer
1. Open the terminal application
2. type `ssh ubuntu@<ip_address>` (replace <ip_address> with the ip address of your CLIMB machine.
3. Enter your password when prompted

### Transferring data to your machine

There are a variety of options for transferring data to your machine in the cloud (actually Warwick University which is in an unglamorous city in England called Coventry).

**galaxy** - If you are using Galaxy, it has an inbuilt way of uploading data that will be covered by any online introductory tutorial.

**`scp`**  - if you choose this option I assume you already know what you are doing

**FileZilla** - to transfer so that you can manipulate data on the command line on your cloud machine. You can’t reliably transfer large files over the web (i.e. HTTP, hyper text transfer protocol) so we use an alternative ‘type’ of internet called FTP (file transfer protocol). In exactly the same way that you have HTTP browsers for looking at the web, like Chrome and Internet Explorer, you have FTP ‘browsers’ for transferring data. FileZilla is the most popular of these browsers.

1. Download [FileZilla] client
2. When you open filezilla, you should see this, without my coloured annotations. ![](https://dl.dropboxusercontent.com/u/24396862/fz1.png)
3. After you click on the little button highlighted in the above (the one that says ‘click on this’ next to it). Follow the instructions on the below diagram ![](https://dl.dropboxusercontent.com/u/24396862/fz2.png)
4. Then (first time only): ![](https://dl.dropboxusercontent.com/u/24396862/fz3.png)
5. Then you can navigate through your filesystem on the lefthand (local computer from 2b) side and drag and drop onto the right hand side (remote computer from 2b), or vice versa. Info on transfer time will be available in the ‘info about transfer time’ box from 2b.



[the galaxy project wiki]: https://wiki.galaxyproject.org/Learn
[ABPRI]: http://sepsis-omics.github.io/tutorials/
[putty]: http://www.putty.org/
[mputty]: http://ttyplus.com/multi-tabbed-putty/
[FileZilla]: https://filezilla-project.org/
