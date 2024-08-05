## To make a shell fully functional here are the steps you would need to follow:

use 
```
python3 -c 'import pty; pty.spawn("/bin/bash")'
```

now you will get a better functioning shell but still it would lack the capabilites to use `clear` like commands hence you will need to use this command

```
export TERM=xterm
```

now still upong pressing `ctrl + C` you would still lose the shell to avoide that press `ctrl + z` to background the shell and then use the command to bring up the shell:

```
stty raw -echo;fg
```

Now you will have a fully functioning shell which youo could use
