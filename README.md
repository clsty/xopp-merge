# xopp-merge
The python scripts merge multiple [Xournalpp](https://github.com/xournalpp/xournalpp)'s note file `*.xopp` into one.

# Usage
On most Linux distros, run `./install` to copy scripts to `/usr/bin/`, and run `./uninstall` to remove them.

Then you can directly use these scripts in shell.

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

# History
It's originally from <https://github.com/friciwolf/XournalppUtils>, and modified as <https://github.com/AyushmaanAggarwal/XournalppUtils>.

For more info, see
- <https://github.com/xournalpp/xournalpp/issues/2474>
- <https://github.com/xournalpp/xournalpp/issues/2816>
