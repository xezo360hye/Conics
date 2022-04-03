# What is Conics?

Conics `(CONsole comICS)` is a program that helps you watch comics from `xkcd.com` right in your TTY, without even starting the X server!


# Installation

## Dependencies

Conics requires FBI or FIM to display images using framebuffer, so you need one or both installed

Arch (FIM is in AUR):

```
sudo pacman -S fbida
yay -S fim
```

Debian, Ubuntu and derivatives:

`sudo apt-get install fbi fim`

Other:

Idk, please tell me if you know

## Project

Run the following commands to install this program:

```
# Download
git clone https://github.com/xezo360hye/Conics

# Make it executable
chmod +x Conics/conics

# Move to $PATH
sudo mv Conics/conics /usr/local/bin/

# Clean up
rm -rf Conics
```

This will do all the job needed

*If you don't have root access, instead of 3rd command run `mv Conics/conics ~/.bin/conics` or move that file to wherever you have acces in $PATH*

# Usage

To get help message use `conics -h` or `conics --help` - there's all you need to know about arguments

To navigate through downloaded images, use `J` and `K` keys, or `space` to move forward UNTIL THE LAST ONE REACHED. Press `H` in FBI to get more info

# Options

## Dir (-d)

Use to specify the directory where downloaded images will be stored - for example, `~/Pictures` or `.hidden_memes`. Default folder is *.* (current working directory)

## Format (-f)

Format is used in `mktemp` command, so check it for more information. It needs to end with 3 or more X's that will be replaced with random ~letters and numbers~ alnums. By default format is *img-XXXXX*

## Count (-c)

Count of comics you want to see. If not used, only one will be shown *(have you done your homework yet?)*

## Time (-t)

Great feature of FBI: if you don't press any key in ARG seconds, it automatically goes to the next one

## Remove (-r)

To remove files after closing FBI / FIM. By default it's false, use this flag to change to true

## Viewer (-w)


