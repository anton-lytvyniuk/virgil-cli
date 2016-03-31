NAME
====

**keygen** -- generate Private Key with given parameters

SYNOPSIS
========

**virgil keygen** \[-o <file>\] \[-a
<bp256r1|bp384r1|bp512r1|secp192r1|secp224r1
           |secp256r1|secp384r1|secp521r1|secp192k1|secp224k1|secp256k1
           |rsa3072|rsa4096|rsa8192>\] \[-p <arg>\] \[-V\] \[--\]
\[--version\] \[-h\]

DESCRIPTION
===========

Generate Elliptic Curve Private Key or RSA Private Key.

OPTIONS
=======

    -o <file>,  --out <file>
     Private key. If omitted, stdout is used.

    -a <bp256r1|bp384r1|bp512r1|secp192r1|secp224r1|secp256r1|secp384r1
      |secp521r1|secp192k1|secp224k1|secp256k1|rsa3072|rsa4096|rsa8192>,
      --algorithm <bp256r1|bp384r1|bp512r1|secp192r1|secp224r1|secp256r1
      |secp384r1|secp521r1|secp192k1|secp224k1|secp256k1|rsa3072|rsa4096
      |rsa8192>
     Generate elliptic curve key or RSA key with oneof the following
     positions:

        * bp256r1 - 256-bits Brainpool curve;

        * bp384r1 - 384-bits Brainpool curve;

        * bp512r1 - 512-bits Brainpool curve;

        * secp192r1 - 192-bits NIST curve;

        * secp224r1 - 224-bits NIST curve;

        * secp256r1 - 256-bits NIST curve;

        * secp384r1 - 384-bits NIST curve (default);

        * secp521r1 - 521-bits NIST curve;

        * secp192k1 - 192-bits "Koblitz" curve;

        * secp224k1 - 224-bits "Koblitz" curve;

        * secp256k1 - 256-bits "Koblitz" curve;

        * rsa3072 - 3072-bits "RSA" key;

        * rsa4096 - 4096-bits "RSA" key;

        * rsa8192 - 8192-bits "RSA" key

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

1.  Generate Elliptic 384-bits NIST Curve Private Key(default), your
    password will be requested:

        virgil keygen -o private.key

2.  Generate Elliptic Curve Private Key with password protection:

        virgil keygen -o private.key -p STRONGPASS

3.  Generate Elliptic 521-bits NIST Curve Private Key:

        virgil keygen -o private.key -a secp521r1

4.  Generate RSA Private Key:

        virgil keygen -a rsa8192 -o private.key

SEE ALSO
========

[`virgil(1)`](../markdown/virgil.1.md),  
[`key2pub(1)`](../markdown/key2pub.1.md)