[![Actions Status](https://github.com/genio/alien-sodium/workflows/linux/badge.svg)](https://github.com/genio/alien-sodium/actions)
[![Actions Status](https://github.com/genio/alien-sodium/workflows/macos/badge.svg)](https://github.com/genio/alien-sodium/actions)
[![Actions Status](https://github.com/genio/alien-sodium/workflows/windows/badge.svg)](https://github.com/genio/alien-sodium/actions)

# NAME

Alien::Sodium - Interface to the libsodium library [http://libsodium.org](http://libsodium.org)

# SYNOPSIS

```perl
use strict;
use warnings;

use ExtUtils::MakeMaker;
use Config;
use Alien::Base::Wrapper ();

WriteMakefile(
  Alien::Base::Wrapper->new('Alien::Sodium')->mm_args2(
    ...
    CONFIGURE_REQUIRES => {
      'Alien::Sodium' => '2.000',
    },
    ...
  ),
);
```

# DESCRIPTION

This package can be used by other [CPAN](https://metacpan.org) modules that
require [libsodium](http://libsodium.org).

# SEE ALSO

- [libsodium](http://libsodium.org)

# AUTHOR

Alex J. G. Burzyński <`ajgb@cpan.org`>

# CONTRIBUTORS

Graham Ollis <`plicease@cpan.org`>

# COPYRIGHT & LICENSE

Copyright (c) 2015 Alex J. G. Burzyński. All rights reserved.

This program is free software; you can redistribute it and/or modify it
under the same terms as Perl itself.
