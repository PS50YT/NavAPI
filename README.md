# Nav API

<img src='https://cdn.modrinth.com/data/cached_images/33fe78120b6bba45a1727ffc380744dad992dd65.png' alt='icon' height='180px' weight='180px'>
<br><br>

## <a href='https://www.spigotmc.org/resources/navapi.139103/'>[![Nav API SpigotMC](https://img.shields.io/badge/NavAPI-Spigot-yellow?style=for-the-badge&logo=https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSW8EAqEiKCkEgSo3B1FgaEFBhF16nzwRhqzqaorZuaPilXyVM4mN1KwvBK&s=10)](https://www.spigotmc.org/resources/navapi.139103/) <a href='https://github.com/PS50YT/NavAPI'>[![Nav API GitHub](https://img.shields.io/badge/NavAPI-GitHub-black?style=for-the-badge&logo=https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSW8EAqEiKCkEgSo3B1FgaEFBhF16nzwRhqzqaorZuaPilXyVM4mN1KwvBK&s=10)](https://github.com/PS50YT/NavAPI)  <a href='https://modrinth.com/plugin/navapi'>[![Nav API Modrinth](https://img.shields.io/badge/NavAPI-Modrinth-green?style=for-the-badge&logo=https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSW8EAqEiKCkEgSo3B1FgaEFBhF16nzwRhqzqaorZuaPilXyVM4mN1KwvBK&s=10)](https://modrinth.com/plugin/navapi) 

NavAPI is a lightweight API and library for Minecraft mods that configure, integrate with, or modify the behavior of other mods. NavAPI fixes or reduces bugs and problem caused due to the modified mod. NavAPI is designed to make mod development simpler and more compatible, while keeping it great in performance.

## What is NavAPI?

NavAPI is an API and Library for mods which configures other mods. This mod basically prevent the game from various bug occured due to the mod's configurations and functions.

## Why I need this API

If you made a mod which configures other mods then this API is for you. This mod reduces many bugs which occured when you make a new mod which edits another mod.

## Advantages of NavAPI

- 🏷️ Available for almost every Minecraft versions and modloaders.
- 🐞 Fixes or reduces many bugs caused due to configuration of other mods.
- 🪶 Lightweighted API.
- 🧩 Also available in form of Plugins.
- 🌐 Can be used in servers.
- 🧱 Supports all mods.
- 🔒 Forces your modification.

![mod menu look](https://cdn.modrinth.com/data/cached_images/2263ba5caba52978732f445531a5d4afbf674988.png)

## 📦 For Developers

1. Developers would have to add dependency of this API and have to 

2. Compile the mod in ```.jar``` extension

3. Extract compiled file
   
4. Create a folder inside the extracted folder ```/navapi-lib```
   
5. Inside ```/navapi-lib``` create a file ```navapi-connect.properties.kts```.

6. <b> Inside ```navapi-connect.properties.kts```

```
navapi.code.style=official
api.name = "navapi"

import Connector-api.properties

fun main() {
    code("\api-lib\initialize.settings.gradle".versionNonNull > "api-load".version)
    code("\online\navapi\navapi.class".versionNonNull > "build".version)

extract architectury-loom-fix.zip

import architectury-loom-fix\architectury-loom-1.17\src

package architectury-loom-fix.architectury-loom-1.17.src

architectury-loom {
       fun initialize() {
       architectury-api:true
    }
}

Base=NavAPI
type="vulkan"
path: "roots.json"
type: 'vulkan'
extra : (
vulkan-handler : true
vulkan-version : *
)
OpenGL : "opengl.java","https://www.opengl.org/"
}
```

7. Compress the file into ```.jar``` extension
