# Install Mac OS X 10.11 El Capitan Dev Tools

0. First invocation of git invokes this dialog:

![git](git_install.png)

0. Choose *install* to install command line utilities
0. Install brew
        ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
0. Install atom
        brew install Caskroom/cask/atom
0. Install python 3
        brew install python3
0. Install virtualenv
        pip install virtualenv
0. Install virtualenv wrapper
        pip install pyenv-virtualenvwrapper
0. Edit ~/.bash_profile
        alias python=python3

        export WORKON_HOME=~/Environments
        export PROJECT_HOME=~/Source
        export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3
        export VIRTUALENVWRAPPER_VIRTUALENV=/usr/local/bin/virtualenv
        export VIRTUALENVWRAPPER_VIRTUALENV_ARGS='--no-site-packages'

        source /usr/local/bin/virtualenvwrapper.sh
