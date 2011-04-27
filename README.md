# Jumplist - Bookmarks For Bash
*Beta. Haven't tested on other systems yet, but should work fine :)*

## Usage
Add the current directory to your Jumplist by giving it a key: `jump add newproject`

You can now jump to it at any time: `jump to newproject`

Delete a location from your Jumplist with: `jump delete newproject`

Or view all locations in your Jumplist with: `jump list`


## Installation
Copy `jumplist-driver` into your home directory as `.jumplist-driver`:

	cp ./jumplist-driver ~/.jumplist-driver

Copy `jumplist-worker` to somewhere in your PATH (eg. `/usr/local/bin/`):

	cp ./jumplist-worker /usr/local/bin/jumplist-worker

And give it execute permissions:

	chmod +x /usr/local/bin/jumplist-worker

Add the following to your `~/.bashrc`:

	source ~/.jumplist-driver

And create a settings file for Jumplist to use:

	touch ~/.jumplistrc


## Advanced Usage
A shorter syntax for jumping to a directory is:

	jump newproject

Is typing `jump` too long? Add the following to your `~/.bashrc`:

	alias j="jump"

You can now:

	j newproject
	j add secondproject
	j list

A full collection of aliases could be:

	alias j="jump"
	alias jl="jump list"
	alias ja="jump add"
	alias jd="jump del"

Ubër fast jumping:

	ja proj  # Add current directory as 'proj'
	j proj   # At any other time, jump to the directory tagged 'proj'
	jl       # View all directories in your jumplist
	jd proj  # Delete the directory tagged 'proj' from your jumplist
