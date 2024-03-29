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

-Clone My_Doc repository
```
cd ~/Documents/git
git clone git@github.com:philliple0610/My_Doc.git
```

### Setup Java

```
sudo dnf install java-1.8.0-openjdk
```
-Check java
```
java --version
```
### Setup Minecraft
-Link: https://fedoramagazine.org/play-minecraft-fedora/

-Download Minecraft.jar from https://minecraft.net/en-us/download/

#### Backup my Minecraft
```
cd
tar -czvf .minecraft.tar.gz .minecraft
tar -czvf minecraft.tar.gz minecraft
cp .minecraft ~/Documents/git/My_Files/
cp minecraft ~/Documents/git/My_Files/
cd ~/Documents/git/My_Files/
git status
git add -A
git commit -am "Blah Blah Blah"
git push
```
#### Get my minecraft files
```
cd ~/Documents/git
git clone git@github.com:philliple0610/My_Minecraft.git
cd -r ~/Documents/git/My_Minecraft/minecraft ~/
cd -r ~/Documents/git/My_Minecraft/.minecraft ~/
```
-Make a directory for Minecraft (first time only)
```
mkdir ~/minecraft
cp ~/Download/Minecraft.jar ~/minecraft/
```
-Do this when your done (to open Minecraft)
```
cd ~/minecraft/ 

java -jar Minecraft.jar
```
