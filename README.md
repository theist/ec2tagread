NAME
    ec2tagread - Check tags from an ec2 instance

SYNOPSYS
    ec2tagread --list

    ec2tagread --all

    ec2tagread --json

    ec2tagread --help

    ec2tagread <tag>

DESCRIPTION
    ec2tagread list or return tag values within an EC2 instance (ubuntu/debian
    atm.), it requres ''ec2metada'' executable and botocore library. It uses
    current instance''s id to get tags, so it cannot be used for check tags for
    arbitrary instance ids or be used outside an AWS instance. Instance or
    active IAM User must be capable of read tags either by aws credentials or
    IAM instance roles (EC2 DescribeTags permission). The default region is eu-west-1,
    you can change the region using the AWS_DEFAULT_REGION environment variable.

PARAMETERS
    --list
        list all available tags

    --all
        list all tags and values on a human readable way

    --json
        list all tags and values in a json array

    --help
        shows this help text

    <tag>
        returns the value of the specified tag


AUTHOR
    Carlos Peñas San José <https://github.com/theist>

COPYRIGHT
    Copyright ©2016 The Cocktail Experience S.L.U

    Lic. GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>

    This is free software: you are free to change and redistribute it. There is
    NO WARRANTY, to the extent permitted by law.

