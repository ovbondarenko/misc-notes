# Basic SSH access setup

* Go to home directory
* In command line, type `cd .ssh` or `mkdir .ssh` and then `cd .ssh` if the folder does ot exist
* Create a new ssh key using `ssh-keygen -t rsa`
* Accept the default filename (`id_rsa`)
* Can leave passphrase blank
* Copy the public ssh key `id_rsa.pub`:
    * `cat id_rsa.pub`
    * copy the **entire** string
* Add it to your Github or Gitlab account (Settings --> SSH Keys)
* Test connection using by running `ssh -vvvT git@github.com` in command line
