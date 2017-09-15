# Playing with black box
```bash

brew install blackbox gpg
gpg --gen-key
gpg --list-secret-keys --fingerprint | grep --color=auto '[0-9A-F]\{4\}$'
```
Now take the hopefully colored last 4 digits of hex
```bash
export MY_KEY_ID=`those 4 digits`
gpg --keyserver pgp.mit.edu --send-keys $MY_KEY_ID
```

Then let me know which email you used and send me that to me.

