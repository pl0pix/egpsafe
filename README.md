# egpsafe -- Eriks Gpg Password Safe

# Motivation
The goal of this script is to store passwords in a file without any format
and keep it as secure as possible. This means gpg encrypted. It must still
work, if most other things on a host do not work anymore. This means: egpsafe
should have least possible dependencies. That's why it has a command line
interface and no gui.

# Features
 * depends only on bash, vi and gpg (in offline mode)
 * mutiple gpg recipients possible. eg. you have seperate keys for work/private
 * sync password safe to hup (adds a dependency to ssh)
 * uses wipe if TMPFILE is located on a harddrive

# Modes
 * offline (default) no synchronisation happens. submodes: edit/see/search
 * online/merge sync in either direction: hup or spoke

# Tested Operating Systems
 * Debian Linux
 * Ubuntu Linux
 * MacOS 10.6

### Search mode
 * please think about setting "set ignorecase" in vi.

### Merge mode
 * this mode is not extensivly tested.

 -- Erik Wenzel <erik@code.de>, So 12 Dez 2010 01:56:22 CET
