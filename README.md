# NAME

dnslg - A command line interface to the dns-lg DNS Looking Glass service.

# USAGE

    dnslg OPTIONS | [QNAME [QTYPE]]

# ARGUMENTS

- --help

    Display this help message

- QNAME

    Fully-qualified domain name to query. Defaults to EXAMPLE.COM

- QTYPE

    Query type. Defaults to A.

# OUTPUT

For each available node, `dnslg` will output the response received in presentation format. Example:

    $ dnslg xyz SOA
    Response from ch01 (Swiss Privacy Foundation, Switzerland, AS13030):

        xyz. 3185 IN SOA ns0.centralnic.net. hostmaster.centralnic.net. 3000170814 900 1800 6048000 3600

    Response from ch02 (Swiss Privacy Foundation, Switzerland, AS13030):

        xyz. 3186 IN SOA ns0.centralnic.net. hostmaster.centralnic.net. 3000170814 900 1800 6048000 3600

# LICENSE

This program is Free Software; you can use it and/or modify it under the same terms as Perl itself.

# COPYRIGHT

Copyright 2015 CentralNic Group plc.

# SEE ALSO

- [http://www.dns-lg.com](http://www.dns-lg.com)
- [https://www.centralnic.com](https://www.centralnic.com)
