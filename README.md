settings-sharelatex
===================

A small module to allow global config settings to be set for all services
within the ShareLaTeX architecture.

Settings file location
----------------------

You can specify a custom location for the settings file by setting the
`SHARELATEX_CONFIG` environment variable. E.g.

	$ export SHARELATEX_CONFIG=/home/james/config/settings.development.coffee

Otherwise, the settings will be loaded from `config/settings.NODE_ENV.coffee`,
where `NODE_ENV` is another evnironment variable, or defaults to `development`.

The config directory is first looked for in the current directory, and then relative
to the settings module directory.