Done on Linux. I am not including instructions on installing linux here.

1.) Creating a Git Account.
Go Here: https://github.com/
Click "Sign Up"
Create a user name and password.
Get teacher to add you to the class group.

2.) Installing Git to my personal machine
Open the terminal.
Do: sudo apt-get install git

3.) Cloning a directory to my pc, and uploading it to my personal git account.
Open the terminal.
Do: git clone https://github.com/unh-comp-698-systems-software/notes.git
Do: cd notes
Do: git remote add vitali https://github.com/CrazyDiamond567/Systems_Software_Setup_Notes
Do: git remote
we should see "origin" and "vitali"
Do: git add *
Do: git commit -a -m "message goes here"
Do: git push vitali master

4.) Installing Docker
Open the terminal.
Do: sudo apt-get update
Do: sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
Do: sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-xenial main'
Do: sudo apt-get update
Do: sudo apt-get install -y docker-engine
Do: docker
If you get help information, it works.
