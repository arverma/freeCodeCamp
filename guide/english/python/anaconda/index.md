---
title: Anaconda
---
**Anaconda** is an environment manager for Data Science and related areas. It has a collection of numerous packages that comes preinstalled and managed by ``conda``. However one can also use ``pip`` inside Anaconda.
Anaconda easily creates, saves, loads and switches between environments on your local computer. It was created for Python programs, but it can package and distribute software for any language.
Conda as a package manager helps you find and install packages. If you need a package that requires a different version of Python, you do not need to switch to a different environment manager. With just a few commands, you can set up a totally separate environment to run that different version of Python, while continuing to run your usual version of Python in your normal environment.
 It is platform-agnostic, so you can use it whether you are on Windows, macOS or Linux.


## Overview

The quickest way to start using conda is to go through the
20-minute [Getting started with conda](https://conda.io/docs/user-guide/getting-started.html) guide.

The ``conda`` command is the primary interface for managing
installations of various packages. It can:

* Query and search the Anaconda package index and current
  Anaconda installation.

* Create new conda environments.

* Install and update packages into existing conda environments.

## Examples

```
Update conda in your default environment 
  $ conda upgrade conda
  $ conda upgrade --all

Create a new environment with conda
  $ conda create -n [my-env-name]

Activate the environment you created
  $ source activate [my-env-name]

Take a look at the environment you created
  $ conda info
  $ conda list

Install a package with conda and verify it's installed
  $ conda install numpy
  $ conda list

Take a look at the list of environments you currently have
  $ conda info -e

Remove an environment
  $ conda env remove --name [my-env-name]
```
TIP: You can abbreviate many frequently used command options that are preceded by 2 dashes (--) to just 1 dash and the first letter of the option. So --name and -n are the same, and --envs and -e are the same.

For full usage of each command, including abbreviations, see
[Command reference](https://conda.io/docs/commands.html) and [Cheat Sheet](https://kapeli.com/cheat_sheets/Conda.docset/Contents/Resources/Documents/index) for ``conda`` commands.


### Sources
1. [Anaconda Documentation](https://docs.anaconda.com/)
2. [Conda Documentation](https://conda.io/docs/)
3. [Conda commands](https://medium.com/@margaretmz/anaconda-jupyter-notebook-tensorflow-and-keras-b91f381405f8)
