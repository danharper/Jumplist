Copy `jumplist-driver` into your home directory as `.jumplist-driver`

Copy `jumplist-worker` to somewhere in your PATH (eg. /usr/local/bin/)
And give it execute permissions with `chmod +x jumplist-worker`

Add the following to your `~/.bashrc`:
	source ~/.jumplist-driver

Jumplist will create a `.jumplistrc` file in your home dir to store your Jumplist
