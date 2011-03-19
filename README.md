Copy `jumplist-driver` into your home directory as `.jumplist-driver`
	cp ./jumplist-driver ~/.jumplist-driver

Copy `jumplist-worker` to somewhere in your PATH (eg. /usr/local/bin/).
	cp ./jumplist-worker /usr/local/bin/jumplist-worker

And give it execute permissions:
	chmod +x /usr/local/bin/jumplist-worker

Add the following to your `~/.bashrc`:
	source ~/.jumplist-driver

And create a settings file for Jumplist to use:
	touch ~/.jumplistrc

Jumplist will create a `.jumplistrc` file in your home dir to store your Jumplist
