# snip

## example
```sh
echo stdin | snip -l shell
```
will output
```sh
while read -r line; do
	echo "$line";
done;
```

## useful trick in vim
create a file and type
```sh
init
stdin
```
and hit `!ipsnip`. You will get
```sh
#!/bin/sh

title='XXX'
usgmsg='XXX'

while read -r line; do
	echo "$line";
done;
```

`!ipsnip` means: "pipe (`!`) this paragraph (`ip`) to an external program
(`snip`) and replace the output with this paragraph"

## add your custom snippets
open the source code and add another case as you like:
```sh
...

   (shell)

      (greet)
         echo 'hello rotating world from a long sentence';;

...
```

## see also
- [arger](https://github.com/ihsanturk/arger)
