# snip

## example
```
echo stdin | snip -l shell
```
will output:
```
while read -r line; do
	echo "$line";
done;
```
