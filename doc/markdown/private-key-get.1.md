NAME
====

**private-key-get** -- get the Private Key from the Private Key Service

SYNOPSIS
========

**virgil private-key-get** \[-o <file>\] -a &lt;&gt; -f <file> \[-V\]
\[--\] \[--version\] \[-h\]

DESCRIPTION
===========

Get the Private Key from the Private Key Service

OPTIONS
=======

    -o <file>,  --out <file>
     Private Key. If omitted, stdout is used.

    -a <>,  --card-id <>
     (required)  virgil Card identifier

    -f <file>,  --validated-identity <file>
     (required)  Validated identity

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

        virgil private-key-get -a *card_id* -f validated_identity.txt -o private.vkey

SEE ALSO
========

[`virgil(1)`](../markdown/virgil.1.md),  
[`keygen(1)`](../markdown/keygen.1.md),  
[`private-key-add(1)`](../markdown/private-key-add.1.md),  
[`identity-confirm(1)`](../markdown/identity-confirm.1.md)