# "vars.h"
Mini system info: credits to DiabloBlanco! (https://codeberg.org/diabloblanco/)
Mini-library for language C.

# How it helping?
Its giving help if you want to get some user info in your C-Project.

# How to build?
First step: Making config for library:
```bash
$ nano /etc/maldidev/clib/vars.h/varslib.conf
input_type={
    language='C'
    c-include-folder='/usr/include'
    new-lib-name='vars'
    new-lib-format='*.h'
    new-lib-builder='sh'
    new-lib-file='$LIB_FOLD:vars.h'
}
```

Second step: getting vars.sh from repo
```bash
$ git clone https://github.com/maldidev/vars/
```

Third step: changing config
```bash
# in /etc/maldidev/clib/vars.h/varslib.conf:
#   change line 7:
new-lib-file='your-path-to-lib/vars.h'
```

Final step: building
```bash
$ bash vars.sh
```
