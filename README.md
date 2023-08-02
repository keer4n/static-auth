# Static auth

Adds a facet of authentication in a static site.

## Features

- login via an email address
    This creates a new auth file which can br checked securely on client side to authorize access to a file. It authorizes as well as decrypts the file in client using GPG.
    
## Working 

1. Use git-crypt to encrypt a file on git commit.
2. Expose the site via git pages
3. Decrypt on client side using openpgpjs
