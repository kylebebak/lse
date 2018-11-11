# lse (list executables)
a better version of the bash built-in `which`

## usage
imagine you have two versions of `npm` in your `$PATH`. running `lse npm` might return the following:

~~~
lrwxr-xr-x     /usr/local/bin/npm -> ../lib/node_modules/npm/bin/npm-cli.js
lrwxr-xr-x     /usr/local/opt/node@8/bin/npm -> ../lib/node_modules/npm/bin/npm-cli.js
~~~

lse returns all npm executables in your path, in order, with their permissions and their symlinks resolved

## other usage
```
-h            get help (display this page)
-a            list files in every directory in path. after -a, all other options are passed directly to ls, not lse
-l            list all directories in path, without any files
-p            list executables with their full path, one per line
```

## license
This code is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
