# PteroThemes
 Themes for Pterodactyl 1.x

## Will this break my panel? (IMPORTANT)
This will not break your panel unless you use a diffrent theme version for a diffrent panel version, if it for some reason does break your panel it is simple to remove the theme.

## Panel Versioning
Make sure that the theme you are installing corresponds with the version of the panel you are running; no help will be given if you have mismatched versions!

How do i use them?
You simple follow the instructions below, mainly consisting of two or three changes you need to make before you build your panel.

## Install Theme
# User Side
Create a file called main.css in `/var/www/pterodactyl/resources/scripts`

In that file put this text

```@import url(https://oreokitten.github.io/latest/dark-n-purple/user.css);```


After that edit the file index.tsx in /var/www/pterodactyl/resources/scripts

On line 6 at the end of the imports add this

```import './main.css';```
After this build the panel, you can find information of how to do that scroll down

After that just reload your panel and the theme is applied.

# Admin Side
In the file admin.blade.php in `/var/www/pterodactyl/resources/views/layouts/`

On line 36 put the text
```<link rel="stylesheet" href="https://oreokitten.github.io/latest/dark-n-purple/admin.css">```

After this build the panel, you can find information of how to do that scroll down

After that just reload your panel and the theme is applied.

How do i use them?
You simple follow the instructions below, mainly consisting of two or three changes you need to make before you build your panel.


## Rebuild
#Install Dependencies
The following commands will install the necessary dependencies for building your panel.

#Install NodeJS
TIP

You may have to add sudo to the following commands if you are not root.

# Using Nodesource
# Ubuntu/Debian
`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`
`apt install -y nodejs`

# CentOS
`curl -sL https://rpm.nodesource.com/setup_12.x | sudo -E bash -`
`yum install -y nodejs # CentOS 7`
`dnf install -y nodejs # CentOS 8`
By now, you should have NodeJS 12 installed. Make sure this is the case by checking node -v

# Using Node Version Manager(opens new window)
`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash`

`nvm install node`
`nvm alias default node`
`nvm use node`
`node -v` should say 12.20.0 or newer

# Install Yarn and Panel Dependencies
# Install yarn
`npm i -g yarn`

# Now you need to make sure you are in the panel directory
`cd /var/www/pterodactyl`

# Installs panel build dependencies
`yarn install`
#Build Panel
Run this in your panel directory to apply changes (usually` /var/www/pterodactyl`)

# Build panel
yarn build:production

## Enola - 1.2.0, 1.2.1, and 1.2.2
Instructions to install the theme Enola are here
[Enola 1.2.2(Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Enola)
![Preview](./preview/enola.png)


## Twilight - 1.1.3, 1.2.0, 1.2.1, 1.2.2
Instructions to install the theme Twilight are here
[Enola 1.2.2(Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Twilight)
![Preview](./preview/twilight.png)

## Recolor - 1.2.0, 1.2.1, 1.2.2
This theme is a recolor of the panel that you can edit, more information here
[Recolor](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Recolor)

## Dracula - 1.2.0, 1.2.1, 1.2.2
This theme is a recolor of the panel that you can edit, more information here
[Dracula 1.2.2(Latest Panel Version)](https://github.com/OreoKitten/PteroThemes/tree/main/latest/Dracula)
![Preview](./preview/Dracula.png)
![Preview](./preview/Dracula2.png)
## If you have suggestions or issues dm me on discord, Oreo#0949
