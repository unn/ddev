Providers README
================

Providers are connections to external resources that can provide upstream database
or user-uploaded files, for example DDEV-Live, Pantheon.io, and Platform.sh.

The magic to use them goes in a yaml file in this directory.

In general, a db_pull_comand and a files_pull_command must be provided.
By default, they execute inside the web container, and get the full
environment there. If the `environment_variables` stanza is included, then
those variables are populated.

The environment variables provided to custom commands are also available,
see https://ddev.readthedocs.io/en/stable/users/extend/custom-commands/#environment-variables-provided
