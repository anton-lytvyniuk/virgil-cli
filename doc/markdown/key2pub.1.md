NAME
====

**key2pub** -- get Public Key from the Private Key Service

SYNOPSIS
========

**virgil key2pub** \[-i <file>\] \[-o <file>\] \[-p <arg>\] \[-V\]
\[--\] \[--version\] \[-h\]

DESCRIPTION
===========

Get Public Key from the given Private Key

OPTIONS
=======

    -i <file>,  --in <file>
     Private key. If omitted, stdin is used.

    -o <file>,  --out <file>
     Public key. If omitted, stdout is used.

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

        virgil key2pub -i private.key -o public.key


        virgil key2pub -i private.key -o public.key -p STRONGPASS

SEE ALSO
========

[`virgil(1)`](../markdown/virgil.1.md),  
[`keygen(1)`](../markdown/keygen.1.md)