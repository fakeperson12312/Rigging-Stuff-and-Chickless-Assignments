# This is a small guide on how to get websites for free, to access from anywhere. The domains won't be pretty, but they'll work.
```bash
sudo apt-get update && sudo apt-get full-upgrade -y && sudo apt autoremove -y
sudo apt-get install apache2 nginx -y
```
Now, install ngrok. This is the simple way (simplest for me)
```bash
sudo apt-get install snapd -y
sudo snap install ngrok
```
Now, to start ngrok you have to create an account and go to the tab called authtoken and copy and paste the line of code into the bash terminal
Next, start apache2
```bash
sudo systemctl start apache2
```
Then, start ngrok
```bash
ngrok http 80
```
Then, given the link provided, paste that into the search bar and click visit site to see the apache2 index.html file. It's stored in /var/www/html/index.html, so if you want to edit it:
```bash
sudo nano /var/www/html/index.html
```
or
```bash
sudo vim /var/www/html/index.html
```
That's just editing index.html files at that point. If u wanted smth without coding that's free just use google sites or smth
Another way, if you don't want to install ngrok is by using vscode port forwarding, making it public, and copy and pasting the link.
So u might notice there's nginx at the very first thing that's installed. That's another option rather than apache2. U can mess with it urself, im not gonna write it down
Also ngrok is kinda limited, now I prefer **tailscale** it's the best
