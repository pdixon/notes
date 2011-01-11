# Git
## Submodules

To add a submodule to a project:

~~~~{.sh}
git submodule add REPO PATH
~~~~

After cloning a project containing submodules:

~~~~{.sh}
git submodule init
git submodule update
~~~~

To update the submodule:

~~~~{.sh}
cd PATH
git checkout master
git pull
cd -
git commit -am"Updated stuff"`
~~~~

## References

* [Using submodules](http://gaarai.com/2009/04/20/git-submodules-adding-using-removing-and-updating/)
