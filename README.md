![](https://www.baeldung.com/wp-content/uploads/sites/4/2023/04/Password-Cracking.png)

# Azure-Soc-Lab

An Azure Sentinel (SIEM) connected to a live virtual machine acting as a honeypot to lure in real life cyber attackers. We will observe live attacks (RDP Brute Force) from all around the world using a custom PowerShell script to look up attackers Geolocation information and then plot it into Azure Semtinel Map to visualize it!

![](https://github.com/Dsuleodu1/Azure-Soc-Lab/blob/main/Screenshot%202025-06-11%20093403.png)

## Features

- Created with Microsoft Azure Sentinel (SIEM) log analytics.
- Provides Knowledge of KQL, PowerShell scripting, remote desktop protocol and virtual machines.
- No installation necessary just create azure free account ![]().
- Gives you hands on experience dropping firewall rules and creating new users to RDP into.
- Allows you to visualize 24hrs of cyber attacks with precise insights on attackers information.
- Works on Mac, Linux and Windows

## Installation

After install, make sure to run `joe u`. This will download all `.gitignore` files in `~/joe-data/` folder.

### Option 1: Binary

`joe` is available for OSX (macOS), Linux and Windows.

Download the latest binary from the [Releases page](https://github.com/karan/joe/releases). It's the easiest way to get started with `joe`.

Make sure to add the location of the binary to your `$PATH`.

### Option 2: From source

```bash
$ git clone git@github.com:karan/joe.git
$ cd joe/
$ chmod +x tool.sh
$ ./tool.sh build
```

## Usage

### Commands:

```
ls | list       list all available files
u | update      update all available gitignore files
g | generate    generate gitignore files
```

### Basic usage

```bash
$ joe g java    # outputs .gitignore file for java to stdout
```

To update your `.gitignore` files at any time, simply run:

```bash
$ joe u
```

### Overwrite existing `.gitignore` file

```bash
$ joe g java > .gitignore    # saves a new .gitignore file for java
```

### Append to existing `.gitignore` file

```bash
$ joe g java >> .gitignore    # appends to an existing .gitignore file
```

### Multiple languages

```bash
$ joe g java,node,osx > .gitignore    # saves a new .gitignore file for multiple languages
```


### Output

![](https://github.com/Dsuleodu1/Azure-Soc-Lab/blob/main/Screenshot%202025-06-11%20093403.png)

> actionscript, ada, agda, android, anjuta, appceleratortitanium, archives, archlinuxpackages, autotools, bricxcc, c, c++, cakephp, cfwheels, chefcookbook, clojure, cloud9, cmake, codeigniter, codekit, commonlisp, composer, concrete5, coq, craftcms, cvs, dart, darteditor, delphi, dm, dreamweaver, drupal, eagle, eclipse, eiffelstudio, elisp, elixir, emacs, ensime, episerver, erlang, espresso, expressionengine, extjs, fancy, finale, flexbuilder, forcedotcom, fortran, fuelphp, gcov, gitbook, go, gradle, grails, gwt, haskell, idris, igorpro, ipythonnotebook, java, jboss, jdeveloper, jekyll, jetbrains, joomla, jython, kate, kdevelop4, kohana, labview, laravel, lazarus, leiningen, lemonstand, libreoffice, lilypond, linux, lithium, lua, lyx, magento, matlab, maven, mercurial, mercury, metaprogrammingsystem, meteor, microsoftoffice, modelsim, momentics, monodevelop, nanoc, netbeans, nim, ninja, node, notepadpp, objective-c, ocaml, opa, opencart, oracleforms, osx, packer, perl, phalcon, playframework, plone, prestashop, processing, python, qooxdoo, qt, r, rails, redcar, redis, rhodesrhomobile, ros, ruby, rust, sass, sbt, scala, scons, scrivener, sdcc, seamgen, sketchup, slickedit, stella, sublimetext, sugarcrm, svn, swift, symfony, symphonycms, tags, tex, textmate, textpattern, tortoisegit, turbogears2, typo3, umbraco, unity, vagrant, vim, virtualenv, visualstudio, vvvv, waf, webmethods, windows, wordpress, xcode, xilinxise, xojo, yeoman, yii, zendframework, zephir

### BONUS ROUND: Alternate version control software

Joe isn't **just** a generator for `.gitignore` files. You can use it and its output wherever a SCM is used.

```bash
$ joe g java > .hgignore
```

## Tools

#### Bug Reports & Feature Requests

Please use the [issue tracker](https://github.com/karan/joe/issues) to report any bugs or file feature requests.

#### Developing

PRs are welcome. To begin developing, do this:

```bash
$ git clone git@github.com:karan/joe.git
$ cd joe/
$ go run *.go
```

#### `tool.sh`

This is a handy script that automates a lot of developing steps.


```bash
USAGE:
    $ $tool [-h|--help] COMMAND

  EXAMPLES:
    $ $tool deps      Install dependencies for joe
    $ $tool build     Build a binary
    $ $tool run       Build and run the binary
```
