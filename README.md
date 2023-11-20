# xopp-merge
The python scripts merge multiple [Xournalpp](https://github.com/xournalpp/xournalpp)'s note file `*.xopp` into one.

# Usage
On most Linux distros, run `./install` to copy scripts to `/usr/bin/`, and run `./uninstall` to remove them.

Then you can directly use these scripts in shell.

`xopp-mergefolder` will merge `*.xopp` files in alphabetical order.

# Known issues
The script `xopp-merge` seems to be broken.

Similar as [this issue](https://github.com/xournalpp/xournalpp/issues/2474#issuecomment-1265735863).

Error output:
```
Traceback (most recent call last):
  File "/usr/bin/xopp-merge", line 51, in <module>
    pageNb = elements[0].attrib["pageno"]
             ~~~~~~~~~~~~~~~~~~^^^^^^^^^^
KeyError: 'pageno'
```

And the author [said](https://github.com/xournalpp/xournalpp/issues/2474#issuecomment-1312756149):
> The script first looks for the pagenb attributes in the <background> tags (which define a "page" for the script) which are missing for files with built-in background layouts/models (i.e. those without a pdf background, like the attached files). In other words, the script should not skip the <page> tags to work properly.
> Honestly, I should just rewrite it in a complete all-layer-, all-background-supporting and platform-independent way with much cleaner code.
> 
> I really appreciate your work and feedback btw.! I'll see what I can do with the "CLI/offline" solution (unless we want to wrap your solution in an electron app, making it nice, easy-to-use and user-friendly).

# History
It's originally created as <https://github.com/friciwolf/XournalppUtils>, and modified as <https://github.com/AyushmaanAggarwal/XournalppUtils>.

For more info, see
- <https://github.com/xournalpp/xournalpp/issues/2474>
- <https://github.com/xournalpp/xournalpp/issues/2816>
