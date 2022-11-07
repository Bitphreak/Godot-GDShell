# GDShell

<p align="center">
  <a href="https://github.com/Kubulambula/Godot-GDShell">
    <img src="https://github.com/Kubulambula/Godot-GDShell/blob/main/addons/gdshell/docs/logo_text.png" width="700" alt="GDShell logo">
  </a>
</p>


#### ⚠️ This plugin is still in early development


Feature-packed linux-like in-game console for development, debugging, cheats and/or any other interaction with your game.


## 📦 Out of the box
GDShell works right away after installation with no need for a complex setup.

Add you own commands, don't reinvent the wheel and get back to the important stuff that makes your game fun.



## 🏄 Easy to use
Forget creating commands from [`Callable`](https://docs.godotengine.org/en/latest/classes/class_callable.html)s, with messy object and method relations.

Every command is it's own script, resulting in better code organization and project structure by design.


**Just create a script, place it in a command folder and you're good to go!**

```gdscript
extends GDShellCommand
# res://addons/gdshell/commands/hello.gd

func _main(argv, data):
    output("Hello World!")
    return {}
```


## 💪 Simple, yet powerful
Don't let the ease of use fool you. GDShell can be used even for more complex tasks like:

* sequential and conditional command chaining

    `alias cls clear && echo "Success" || echo "Failed"; echo ":("`

* executing commands in background

    `wait_for_godot& ; think_about_your_game_project`

* command result passing

    `gdfetch -s | echo`

The sky is the limit here. Even if you never need any of these features, you can sleep knowing, that they are here, if you ever will.


## 🧩 Modular and customizable
* Do you dislike the default UI?
* Do you wish to have a new operator?
* Do you want to have bunch of buttons that call the commands directly without the console interface?

Every part of GDShell can be modified, extended or replaced as long as you implement the necessary methods.

Nearly anything your heart desire can be done done!


## 🧪 Installation
### Installation via [AssetLib](https://godotengine.org/asset-library/asset/1526)
1. Open AssetLib in your project (AssetLib button in the top center)
2. Search for: **GDShell**
3. Open **GDShell**
4. Click **Download**
5. Click **Install**
6. Go to `Project > Project Settings > Plugins` and check the `Enable` checkbox for GDShell


### Installation via Git
1. **Clone** or **download** the [latest release](https://github.com/Kubulambula/Godot-GDShell/releases/latest)
2. Copy the `gdshell/` folder into your project's `res://addons/` folder.
3. Go to `Project > Project Settings > Plugins` and check the `Enable` checkbox for GDShell


You can also checkout the Godot's [Installing plugins](https://docs.godotengine.org/en/latest/tutorials/plugins/editor/installing_plugins.html) docs


## 📚 Documentation & Tutorials
See the **[Docs](https://github.com/Kubulambula/Godot-GDShell/blob/main/addons/gdshell/docs/docs.md)** page.

For command examples, you can checkout the **[default commands](https://github.com/Kubulambula/Godot-GDShell/tree/main/addons/gdshell/commands/default_commands)**.


## 👥 Contributing
All contributions are very welcome, so feel free to make [issues](https://github.com/Kubulambula/Godot-GDShell/issues), [proposals](https://github.com/Kubulambula/Godot-GDShell/issues/proposal) and [pull requests](https://github.com/Kubulambula/Godot-GDShell/pulls). 


### ❤️ License (It's free, baby!)
GDShell is available under the **MIT license**.
See [`LICENSE.md`](https://github.com/Kubulambula/Godot-GDShell/blob/main/LICENSE.md).

GDShell logo is available under the **Free Art License 1.3**. See [`LOGO_LICENSE.md`](https://github.com/Kubulambula/Godot-GDShell/blob/main/addons/gdshell/LOGO_LICENSE.md)
