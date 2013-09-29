Intro
=====
apt-cyg is a command-line installer for Cygwin which cooperates with Cygwin Setup and uses the same repository. The syntax is similar to apt-get. Usage examples:

    "apt-cyg install <package names>" to install packages
    "apt-cyg remove <package names>" to remove packages
    "apt-cyg update" to update setup.ini
    "apt-cyg show" to show installed packages
    "apt-cyg find|search <pattern(s)>" to find packages matching patterns
    "apt-cyg describe <pattern(s)>" to describe packages matching patterns
    "apt-cyg packageof <commands or files>" to locate parent packages

Available Options:

    --mirror, -m <url> : set mirror (Need x86/x86_64 at the end)
    --cache, -c <dir>  : set cache
    --file, -f <file>  : read package names from file
    --noupdate, -u     : don't update setup.ini from mirror
    --ignore-case, -i  : ignore case distinctions in <patterns> when finding packages
    --help, ?          : shows the usage
    --version          : shows version information

Quick start
===========
First install git through the standard cygwin setup program. Then run the following commands:

    git clone git@github.com:bnormsoftware/apt-cyg.git
    cp apt-cyg/apt-cyg /bin/
    chmod +x /bin/apt-cyg

Or if you will be making changes you can create a symbolic link instead:

    git clone git@github.com:bnormsoftware/apt-cyg.git
    ln -s `pwd`/apt-cyg/apt-cyg
    chmod +x /bin/apt-cyg

Use apt-cyg, for example:

    apt-cyg install nano
