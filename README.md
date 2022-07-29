# Ubuntu-Optimization
Let's renovate our ubuntu by changing everything.

Start by opening your terminal
1. Installing `starship` for changing the look of our terminal

```bash
sudo snap install starship
```
Add `eval "$(starship init bash)"` in the `~/.bashrc` file.
```bash
echo 'eval "$(startship init bash)" ' >> ~/.bashrc
```
> Now exit and restart the terminal and you will see some changes

## Time for Dracula Theme

2. Applying dracula theme on the terminal

Installing `dconf-cli`

```bash
sudo apt-get install dconf-cli -y
```
Cloning to gnome terminal
```bash
git clone https://github.com/dracula/gnome-terminal
cd gnome-terminal
```
Let's run the installation script
```bash
./install.sh
```
**It will ask for some inputs so do the following things** 
* Press **1** and then enter
* Type **YES** and then enter
* Again press **1** and then enter.
* Similarly type **YES** and then enter.
* Finally press **2** and then enter.
Now close the terminal and relaunch it.

3. Applying dracula theme on `gedit`.

Download the raw file 
```bash
wget https://raw.githubusercontent.com/dracula/gedit/master/dracula.xml
```
Now make the `gedit` directory inside the `.local/share/` and inside gedit make a directory called styles move the raw file inside it.
```bash
mkdir ~/.local/share/gedit/
mkdir ~/.local/share/gedit/styles/
mv dracula.xml ~/.local/share/gedit/styles/
```
Now final step is to activate the dracula theme on `gedit`
* So now open the gedit text editor




