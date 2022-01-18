# shellfck
Small bash script to send messages to, or kill, a shell on a linux machine.

## Run
This script needs two flags. An action and a destination. Usage: `bash shellfck [-k|-m] [-a|-s]`

```
-k:	Kill ..
-m:	Message ..		Ex. "Hey how are you"
-a:	.. all pts's
-s:	.. selected pts's	Ex. 1,3,7

-l:	List all connected pts's
-h:	Show help (this screen)
```

For example `bash shellfck -m "hey" -a` will send the string "hey" to all current shells on the machine. Output:

```
[+] Running script

Message send to pts:  0
Ignored own pts:      1
Message send to pts:  3
Message send to pts:  4

[+] Done
```
