ruby-unf_ext
============

Synopsis
--------

* Unicode Normalization Form support library for CRuby

Description
-----------

* Normalizes UTF-8 strings in NFC, NFD, NFKC or NFKD

    # For bulk conversion
    normalizer = UNF::Normalizer.new
    a_bunch_of_strings.map! { |string|
      normalizer.normalize(string, :nfc) #=> string in NFC
    }

* Compliant with Unicode 5.2.0 (for the moment)

Requirement
-----------

* Ruby 1.8.7+, 1.9.2+

* C++ compiler and libstdc++

Installation
------------

	gem install unf

Or:

    ruby extconf.rb && make && make install

Development Resources
---------------------

* http://sourceforge.jp/projects/unf/
* http://sourceforge.jp/ticket/newticket.php?group_id=5256

    For issues regarding files under the directory `unf`, please
    contact this upstream.

* https://github.com/knu/ruby-unf_ext

    The development site and the repository.

License
-------

Copyright (c) 2010 Takeru Ohta
Copyright (c) 2011 Akinori MUSHA

Licensed under the MIT license.
See `LICENSE` for details.
