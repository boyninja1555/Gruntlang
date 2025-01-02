# Gruntlang
![Current Version](https://img.shields.io/badge/Version%201.0.0-brightgreen)
![License](https://img.shields.io/badge/MIT%20License-blue)
Suppose you are transitioning from Scratch and want something simpler than Python? What if you want to embed Python alongside an easier version? Gruntlang does just that!

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)

## Description
Gruntlang is a programming language made for users straight from Scratch or it's text version. Gruntlang is meant to introduce simple CLI tools (known as the green flag and stop sign on Scratch), packages (known as addons or mods on Scratch).

**DISCLAIMER: Gruntlang is not meant for commercial use, but as a learning tool**

## Features
- **A CLI tool** to mimick the green flag and stop sign from Scratch
- **A package manager** to act as a replacement for mods or addons
- **Simple syntax** to prevent a steep learning curve

## Installation

1. Download the [latest release](https://www.github.com/boyninja1555/Gruntlang/releases/latest) installer
2. Open your downloads folder
3. Double-click the EXE/installer
4. Follow the installation steps

## Usage

The file you downloaded was the CLI tool and package manager. You cannot "download a programming language", but you CAN download tools that know what Gruntlang is, such as the official EXE installer you downloaded.
To create your first project, you can either generate one using the CLI or just create a folder named `example-project`, a folder named `src` inside the project folder, and a file named `main.grunt` inside. There are some extra files necessary to tell your tool how to run Gruntlang. Below is the project structure if this was confusing.

```files
> example-project
---> src
------> main.grunt
---> Gruntlang.config
```

Firstly, you need to fill in the `Gruntlang.config`. Notepad works, but you can use any text editor capable of `config` files.

```config
[app]
; Your app's settings
name=Your Project Name
package_name=your_project_name
version=1.0.0

[packages]
; Similar to Scratch's addons or mods, extra tools usable in your code
```

Next, we can finally code. Below is an example file named `main.grunt`.

```gruntlang
; Define variables
var time = 0

; Define a block (aka a "function" in most programming languages)
block main
    ; Add text to the console
    say Hello!

    ; Repeat 10 times (aka a "for loop" in most programming languages)
    repeat 10
        ; Say how many times the loop has done
        say This is the {time} time

        ; Set variable "time" as itself plus 1
        time = time + 1

; Run/use the block "main"
call main
```
