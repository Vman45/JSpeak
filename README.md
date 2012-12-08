h2. JSpeak Demo

http://www.youtube.com/embed/raEUJraXvwY

h2. Installation and Usage

h3. Ubuntu/Debian/Mint:

*Note:* There is a bug in Mint with it's espeak and pulseaudio, not the app itself. However these bugs do not affect the program, and it still opperates just fine and good.

*Note:* Do not copy and paste the *$* at the beginning of the commands or the *#*. The *$* means run as your user. The *#* means run as the root user or use sudo if on an Ubuntu/Mint box.

@$ sudo apt-get install espeak mbrola@

Choose your voices. There are many, but for all english ones, do

@$ sudo apt-get install mbrola-us1 mbrola-us2 mbrola-us3 mbrola-en1@

Many mbrola voices can be installed through apt-get in Ubuntu/Mint. Some such as mbrola-mx1 are not available through apt. If you wish to install those. Follow the manual installation below for them.

h3. Fedora/Suse:

@# yum install espeak@

Fedora and other rpm based systems do not have mbrola and mbrola packages afaik. However this is not a problem. Continue to follow the manual installation for them.

h3. Manual installation of mbrola and mbrola voices (From the espeak/mbrola docs)

*Linux Installation*

From eSpeak version 1.44 onwards, eSpeak calls the mbrola program directly, rather than passing phoneme data to it using a pipe.



1. To install the Linux Mbrola binary, download:
http://www.tcts.fpms.ac.be/synthesis/mbrola/bin/pclinux/mbr301h.zip
Unpack the archive, and copy and rename the file from: @mbrola-linux-i386@ to
@mbrola@ somewhere in your executable path (eg. @/usr/bin/mbrola@ ).



2. Get the en1 voice from:
http://www.tcts.fpms.ac.be/synthesis/mbrola/mbrcopybin.html
Unpack the archive, and copy the *en1* data file (not the whole "en1"
directory) to @/usr/share/mbrola/en1@.

eSpeak will look for mbrola voices firstly in @espeak-data/mbrola@ and then in @/usr/share/mbrola@

*Note:* Get as many voices as you like. Each will show in the voice selection combo box.



3. If you use the eSpeak voice such as "*mb-en1*" then eSpeak will use the mbrola "en1" voice, eg:

@$ espeak -v mb-en1 "Hello world"@

*Note:* This step is just for testing that everything is setup and working correctly.


h3. Obtaining and running the app.

@$ wget https://github.com/downloads/BullShark/JSpeak/JSpeak.tbz@

@$ tar -xf JSpeak.tbz@ 

@$ cd JSpeak@

@$ java -jar JSpeak.jar@

h3. OR Obtain the app from git and run.

@$ git clone git://github.com/BullShark/JSpeak.git@

@$ cd JSpeak/dist@

@$ java -jar JSpeak.jar@

h3. Usage

1. Toggle on the scan button (has a diamond icon). Hover your mouse over other buttons for descriptions.

2. (Optional) Change the voice from the drop down menu of the combo box to set a better sounding mbrola voice.

3. Start copying text from your favorite ebook, the web, email, etc. to begin having the text read to you.

h3. Windows Users:
Install Linux

h3. Help/Support

If you enjoy this software, please consider making a small donation to the programmer, so he can continue to maintain and create new software to help everyday users. Donations can be made the developer's blog, http://linuxinnovations.blogspot.com .