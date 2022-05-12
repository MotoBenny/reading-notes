# [regex python](https://www.datacamp.com/tutorial/python-regular-expression-tutorial)

`import re` - import regular expression

.findall() - returns a list containing all matches
.match() - returns a boolean
.sup( ) - replace one or many matches with a string
.slplit() - returns a list where a sting is split at each match

When i am trying to put together a regex string i use things like google, regexr, and regex101 as my go to tools


## [High Level file operations](https://pymotw.com/3/shutil/)

The shutil module allows you to copy and archive files.

.copyfile() copies the contents of the source file to the destination location, Raises IO error if it lacks the required permission
	* this opens any file for reading, meaning certain file types cannot be copied with this.
	
.copy2() works like copy, but also incliudes logged metadata like accesstime

There are many more file opperations within the shutil module.