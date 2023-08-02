# Static auth

Adds a facet of authentication in a static site.

## Features

- login via an email address
    This creates a new auth file which can br checked securely on client side to authorize access to a file. It authorizes as well as decrypts the file in client using GPG.
    
## Working 

1. Use git-crypt to encrypt a file on git commit.
2. Expose the site via git pages
3. Decrypt on client side using openpgpjs

## Dev server

Any local dev server will work.

For eg., using python 3, a server listening on port 8000 can be started with[^1]:

```shell
    python -m http.server
```

## TODO

- [ ] add dev scripts in a makefile


[^1]: (https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Tools_and_setup/set_up_a_local_testing_server#using_python)[MDN]
