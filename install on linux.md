## Install Ruby using rbenv

1. Ensure all the package dependencies are installed `$ sudo apt install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev dirmngr gnupg apt-transport-https ca-certificates libgdbm-dev autoconf bison`
2. `$ git clone https://github.com/rbenv/rbenv.git ~/.rbenv` to install rbenv.
3. `$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc` then `$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc` activate rbenv auto run on system startups.
4. `$ source ~/.bashrc` to activate in SHELL.
5. `$ git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build` install ruby build.
6. `$ rbenv install -l` executes available ruby list.
7. `$ rbenv install x.x.x` (2.7.0 in this doc for deploying test app) to install a specific version.
8. `$ rbenv versions` to see all the installed versions.
9. `$ rbenv global x.x.x` to activate a version globally.
10. `$ git clone https://github.com/sstephenson/rbenv-vars.git ~/.rbenv/plugins/rbenv-vars` to install rbenv environment variable that is required to setup confedentials info in rbvenv environment variable.

**If we need to uninstall rbenv**

12. `$ rbenv uninstall x.x.x` to uninstall a ruby version.
13. `$ cd ~/.rbenv && git pull` to update rbenv.
14. `$ nano ~/.bashrc` find `export PATH="$HOME/.rbenv/bin:$PATH"` and `eval "$(rbenv init -)"` and remove those line.
15. `$ rm -rf 'rbenv root'` to uninstall rbenv. Login again to make apply.
