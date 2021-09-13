# My Welcome Message plugin for bukkit/spigot Minecraft server

## Features
  Displays a message to the user upon joining. Supports line breaks.

![screenshot](./screenshot.jpg)

- Could display the welcome message, and Op could reload the config 
  
  - `/welcome` to display the welcome message
  - `/welcome reload` to reload the welcome message, (need op)

- support 1.71.1
- support multiple message sections
- support delay display message sections.
  
------

## example of config.yml

config.yml could be find in `\plugins\welcome_plugin\`

```yml
#config.yml
welcome:
    message: '&5Welcome, &r&2%p&r&5 to the Minecraft server! \n Enjoy~~'
    messages:
        - '&3 section1'
        - '&6 section2\ content....'
    linebreak: '\\n'
    delay: 2
```

for message color and format check [Minecraft Formatting code](https://minecraft.gamepedia.com/Formatting_codes).

**todo:** will support multiple line saved in array.

------

## Installation

Download the plugin jar file and put in the plugins folder,
After the first run, you will see the \welcome_plugin\ folder in the plugins
you could update the config.yml to change the welcome message.

## Build the project

### Install Maven

for how to use Maven please read Maven in 5 min:
<http://maven.apache.org/guides/getting-started/maven-in-five-minutes.html>

`mvn install`

The jar will be generated in the target folder. Ex target/welcome_plugin-X.X.X.jar
