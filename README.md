# diary

Script to create diary annotations and explore, visualize and mantain copies of
them. It is possible to create as many diaries as desired and every day is
stored in an individual text-file.

(It has been tried in Ubuntu and Debian)

All the diaries are stored in "~/diary/" and separated folders per each diary
name.

```bash
DIARY_PATH="${HOME}/diary"
```

By default the text editor is vim.

```bash
EDITOR="vim + "
```

For nice visualization of the diary in the web-browser it is recommended to use
markdown syntax. The default web-browser is the default in Ubuntu.

```bash
EXPLORER="sensible-browser"
```

In other Operating Systems you could choose any other web-browser (e.g. firefox).

```bash
EXPLORER="firefox"
```

Show the help
-------------
```sh
diary --help
```

Create or open a diary
----------------------

If is the first annotation of the day it creates a new page. If not, it opens
the actual page (text-file).

```sh
diary name_of_the_diary
```

Show the name of your diaries
----------------------------

```sh
diary -ls
```

or in a list

```sh
diary -lsl
```

Search one sentence
-------------------

If the name of the diary is not specified the sentence is searched in all
the diaries

```sh
diary -s "sentence" name_of_the_diary
```

Explore one diary
-----------------

Visualize all the pages of a diary in a web-browser

```sh
diary -e name_of_the_diary
```

Save your diaries
-----------------

```sh
diary -push
```

Update your diaries
-------------------

```sh
diary -pull
```
