check-tls-certs
===============

Check TLS certificates of domains for expiration dates and more.


Usage
-----

::

    Usage: check_tls_certs [OPTIONS] [DOMAIN]...

      Checks the TLS certificate for each DOMAIN.

      You can add checks for alternative names by separating them with a slash,
      like example.com/www.example.com.

      Exits with return code 3 when there are warnings and code 4 when there are
      errors.

    Options:
      -f, --file FILE              File to read domains from. One per line.
      -v, --verbose / -q, --quiet  Toggle printing of infos for domains with no
                                   errors or warnings.
      --help                       Show this message and exit.

When domains are read from a file, lines starting with a ``#`` are ignored.
