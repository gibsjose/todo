# Todo
Todo is a simple `@TODO` tag tracker. It displays the comment after the tag from all files containing tags, with corresponding file names and line numbers.

For example, a file named `main.c` containing the following tag on line 100:

```
...
__tr_2fv ^= (g_ram & ~(g_ram ^ tr_tt));		//@TODO Use comprehensible variable names
...
```

Becomes:

```
main.c:
		line 100  :	 @TODO  --  Use comprehensible variable names
```

## Installation
```bash
brew tap gibsjose/utils
brew install todo
```

## Usage
```bash
todo [-r] [directory]
```

The optional `-r` option will search the directory recursively for matching files

The optional `directory` is used to specify the directory to search. Defaults to the current directory.
