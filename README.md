# Welcome to GameDeps

Gamedeps verifies dependencies for beginning Linux gamers.  This is a project for Hackweek #13.

## Why?

Games packaged for your Linux distribution are trivial to download and install.  However, Windows games and games not packaged for your distribution are another matter.  For those that can install Linux, but do not have the experience resolving these dependencies, gaming on Linux can be a frustrating affair.

Forums such as WineHQ, GOG and HumbleBundle are wonderful, but can be information overload for the Linux user trying to discern if the tips presented will apply to their system.

The goal of gamedeps is quick gratification of knowing what is missing for a given game with the instructions to resolve those issues.

## Install

Clone the repository.

```
git clone https://github.com/swiftgist/gamedeps/gamedeps.git
```

Install Thor

```
zypper in rubygem-thor
```

## Use

From the command line, run 

```
cd bin
./gamedeps
```

to get a list of games.  Run any of the suggested commands to verify the dependencies for a game.  For instance, run

```
./gamedeps rift
```

to check that RIFT will run.  The output on OpenSUSE 13.2 is 

```
audio:
default-fragments            changed
default-fragment-size-msec   changed
regedit:
StrictDrawOrderingenabled    present
UseGLSLenabled               present
video:
nvidia-gfxG03-kmp-desktop    installed
nvidia                       present
wine:
wine-1.8~rc1                 installed
winetricks:
d3dx9                        installed
d3dcompiler_43               missing     Run "winetricks d3dcompiler_43"
vcrun2008                    installed
vcrun2012                    installed
vcrun2013                    installed
xact_jun2010                 installed
```

## Wiki

See [Wiki](https://github.com/swiftgist/gamedeps/wiki) for more information.



