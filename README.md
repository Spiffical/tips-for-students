# tips-for-students
have any tips for students? share them here!


# Using GitHub with PyCharm

https://www.jetbrains.com/help/pycharm/github.html

# Syncing your code to Compute Canada servers with PyCharm

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
