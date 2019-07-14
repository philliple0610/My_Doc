# Reinstalling My Laptop

### Install Fedora 27

- Insert Fedora 27 Portable USB

- Follow the instructions on the screen and **make yourself as an Administrator**

### Install Chrome

- Open FireFox Browser

- Search for Google Browser and install it

### Setup Git and Github

- Generate SSH Key 
```
ssh-keygen -t rsa -b 4096 -C "philliple0610@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```
**Remember to Store Password**
- Config Git
```
git config --global user.name "Phillip D Le"
git config --global user.email "philliple0610@gmail.com"
git config --list
```
-Signin into github
-Select Settings

-Select SSH and GPG keys
-Select New SSH key

-Copy the content of your workstation machine's ~/.ssh/id_rsa.pub and paste it into the new key
```
vi ~/.ssh/id_rsa.pub
```
-Click on Add SSH key

-Clone my repository
```
git clone git@github.com:philliple0610/My_Doc.git
```




-----------------------------------------------------------------------------------------------------------------------------




Link: https://fedoramagazine.org/play-minecraft-fedora/

sudo dnf install java-1.8.0-openjdk

Check java:
java --version

Download Minecraft.jar from https://minecraft.net/en-us/download/

mkdir ~/minecraft
cp ~/Download/Minecraft.jar ~/minecraft/

cd ~/minecraft
java -jar Minecraft.jar

Running Minecraft on Ubuntu https://www.lynda.com/articles/running-minecraft-ubuntu-linux

Do this when your done (down there)

                                     cd minecraft/ <- first this one

  			  java -jar Minecraft.jar <-then this one
