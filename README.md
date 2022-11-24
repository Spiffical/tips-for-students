# Table of contents
1. [Introduction](#introduction)
2. [Code development](#codedevelopment)
    1. [Working with Git in PyCharm](#git-pycharm)
    2. [Syncing your code to Compute Canada servers in PyCharm](#compute-canada-pycharm)
3. [Miscellaneous](#miscellaneous)

---

## Introduction <a name="introduction"></a>
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
cat /path/to/your/.ssh/public_key.pub
```
Copy the public key, then head over to your chosen Compute Canada server. Paste your public SSH key into the `authorized_keys` file:
```
nano ~/.ssh/authorized_keys
```
In PyCharm, head to `Tools -> Deployment -> Configuration`, and then follow these steps:

1. Click the `+` button, choose `SFTP` to create a new Secure File Transfer Protocol connection, and give it a name, e.g. `cedar`.
2. Click the `...` to add a new SSH configuration
3. In `Host`, type the host information, e.g. `cedar.computecanada.ca`
4. In `Username`, type your username
5. In `Authentication type`, choose `Key pair`
6. In `Private key file`, choose your previously generated private key, e.g. `path/to/your/.ssh/private_key`
7. Test connection! If everything is fine, hit `Okay`
8. Set the `Root path` to your Compute Canada server (might be easiest to `Autodetect`)
9. Head to the `Mappings` tab, and choose a folder on your Compute Canada server to deploy your code to
10. Finally, click on the SFTP server name you made, and click the checkmark to select it as the default

Now you can deploy your code to Compute Canada by selecting `Tools -> Deployment -> Upload to <name>`

You can also enable auto-deployment everytime you save by selecting `Tools -> Deployment -> Automatic upload`

---

## Miscellaneous <a name="miscellaneous"></a>

Organize your tabs with [OneTab](https://chrome.google.com/webstore/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall?hl=en) (if using Chrome)


