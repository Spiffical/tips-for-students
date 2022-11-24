# Table of contents
1. [Introduction](#introduction)
2. [Code development](#codedevelopment)
    1. [Working with Git in PyCharm](#git-pycharm)
    2. [Syncing your code to Compute Canada servers in PyCharm](#compute-canada-pycharm)
3. [Miscellaneous](#miscellaneous)

---

## This is the introduction <a name="introduction"></a>
This is a repository of all the helpful tools that various students have used to make their lives better. Enjoy!

---

## Code development <a name="codedevelopment"></a>
Optimizing your coding efficiency with convenient tools

### Working with Git/GitHub in PyCharm <a name="git-pycharm"></a>
https://www.jetbrains.com/help/pycharm/github.html

### Syncing your code to Compute Canada servers in PyCharm <a name="compute-canada-pycharm"></a>
If you don't have an SSH key, execute the following command in your local terminal:
```
ssh-keygen
```
then print out the contents of your newly generated public SSH key:
```
cat /path/to/your/public_key.pub
```
Copy the public key, then head over to your chosen Compute Canada server. Paste your public SSH key into the `authorized_keys` file:
```
nano ~/.ssh/authorized_keys
```

---

## Miscellaneous <a name="miscellaneous"></a>

Organize your tabs with [OneTab](https://chrome.google.com/webstore/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall?hl=en) (if using Chrome)


