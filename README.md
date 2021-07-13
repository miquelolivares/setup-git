# setup-git
setup git (copied from @abourget getting-started-with-golang repository)

Install Git
-----------

Download from:

* http://git-scm.com/downloads

Setup GitHub authentication
---------------------------


### Generate a new key

Run:

    cat $HOME/.ssh/id_rsa.pub

If you see `No such file or directory`, continue on, otherwise skip
this `ssh-keygen` step and go to `Register your key on GitHub`.

Still in "Git Bash", run:

    ssh-keygen

Accept the default file name (hit ENTER).  This key gives access to
all your github repos. Secure it with a password when asked.

  * This password never leaves your computer, the key shouldn't
    either, but if lost, it is encrypted with this password.


### Register your key on GitHub

Run:

    cat $HOME/.ssh/id_rsa.pub

Go to:

* https://github.com/settings/ssh

Click "Add SSH key" (at the top right of the box).

Copy the `ssh-rsa .......` in the `Key` input field. Don't fill in
`Title` (it will use the key comment).

GitHub will ask you to confirm with your GitHub password.
