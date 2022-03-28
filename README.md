# What is Conics?

Conics `(CONsole comICS)` is a program that helps you watch comics from `xkcd.com` right in your TTY, without even starting the X server!


# Installation

## Step 1 - dependencies

Conics uses FBI (**F**rame**B**uffer **I**mageviewer) and cURL so install them

Arch (FBI is in AUR):

`yay -S curl fbida`

Debian, Ubuntu, Mint:

`sudo apt-get install fbi`

Other:

Idk, please tell me if you know

## Step 2 - main

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

And you are done!

# Usage

## General

To get help message use `conics -h` or `conics --help` - there's all you need to know about arguments

To navigate through downloaded images, use `J` and `K` keys, or `space` to move forward UNTIL THE LAST ONE REACHED. Press `H` in FBI to get more info

## Options

### Dir (-d)

Use to specify the directory where downloaded images will be stored - for example, `~/Pictures` or `.hidden_memes`. Default folder is *.* (current working directory)

### Format (-f)

Format is used in `mktemp` command, so check it for more information. It needs to end with 3 or more X's that will be replaced with random ~letters and numbers~ alnums. By default format is *img-XXXXX*

### Count (-c)

Count of comics you want to see. If not used, only one will be shown *(have you done your homework yet?)*

### Time (-t)

Great feature of FBI: if you don't press any key in <> seconds, it automatically goes to the next one. Closes when reached to the end

### Remove (-r)

Use it with or without argument. If next arg after -r is `true` or `false`, conics uses it, but if not it'll set it to *true*. However, the default value is *false*