# ejabberd-mod-mam

**ejabberd-mod-mam** is a module for the ejabberd XMPP server that implements
the "Message Archive Management" functionality [XEP-0313][xep-0313] and "Result Set Management" [XEP-0059][xep-0059] using a
[Redis][redis] backend.

## Install

Copy and paste mod_mam_redis.erl to your working directory.


## Configuration

In order to use **mod-mam** you have to add it to the modules section in your
`ejabberd.yml`. This could look like this:

``` yaml
modules:
  ...
  mod_mam:
    db_type: redis
    default: always
  ...
```


## Maintainer

*mod_mam_redis* is written by sngyai. You can reach me at
<progyang@gmail.com>.


[xep-0313]: http://xmpp.org/extensions/xep-0313.html
[xep-0059]: http://xmpp.org/extensions/xep-0059.html
[redis]: http://redis.io
