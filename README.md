# Okta CLI

Whalebrew packaging for https://github.com/flypenguin/okta-cli

The current featureset is purely based on the author's needs, which currently are:

* list users (using API `search=` and `query=` functionality, and local filtering)
* update users

## Requirements

Requires whalebrew https://github.com/whalebrew/whalebrew

To install it:

`brew install whalebrew`

Or visit the whalebrew releases page https://github.com/whalebrew/whalebrew/releases

## Quickstart

```bash
$ whalebrew install tjamet/okta
$ okta config new -n my-profile -u https://my.okta.url -t API_TOKEN
$ okta users list -f 'email eq "my@email.com"'
$ okta users update id012345678 --set email=my@other.email.com --set phone=01234/5678
```

