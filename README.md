# yesno - Bash Yes/No prompt with customizable question and default response.

I found myself needing this often, so here it is. Asks a yes or no question and exits with 0 (yes) or 1 (no) depending on the answer.

## Installation

```
sudo cp yesno /usr/bin/
```

## Usage

simple usage, by exit code:

```
$ yesno && echo "do this only if answer is yes"
Confirm? [y/n]:
```

or by return value:

```
$ IS_CONFIRMED=$(yesno)
Confirm? [y/n]:y
$ echo $IS_CONFIRMED
yes
```


Customizable prompt and default answer:

```
$ yesno "do the thing?" 'y' && do_the_thing.sh
do the thing? [Y/n]:
```



