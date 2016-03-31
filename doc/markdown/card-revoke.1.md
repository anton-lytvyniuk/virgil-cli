NAME
====

**card-revoke** -- revoke Card from the Public Keys Service

SYNOPSIS
========

**virgil card-revoke** -a <arg> \[-f <file>\] -k <file> \[-p <arg>\]
\[-V\] \[--\] \[--version\] \[-h\]

DESCRIPTION
===========

Revoke a Card from the Public Keys Service

OPTIONS
=======

    -a <arg>,  --card-id <arg>
     (required)  virgil Card identifier

    -f <file>,  --validated-identity <file>
     Validated identity

    -k <file>,  --key <file>
     (required)  Private key

    -p <arg>,  --private-key-password <arg>
     Password to be used for Private Key encryption.

    -V,  --VERBOSE
     Show detailed information

    --,  --ignore_rest
     Ignores the rest of the labeled arguments following this flag.

    --version
     Displays version information and exits.

    -h,  --help
     Displays usage information and exits.

EXAMPLES
========

1.  Revoke Virgil Card with a confirmed identity:

        virgil card-revoke -a *card_id* -f *validated-identities.txt -k private.key

2.  Revoke Virgil Card with a confirmed identity:

        virgil card-revoke -a *card_id* -k private.key

SEE ALSO
========

[`virgil(1)`](../markdown/virgil.1.md),  
[`card-create(1)`](../markdown/card-create.1.md),  
[`public-key-revoke(1)`](../markdown/public-key-revoke.1.md)