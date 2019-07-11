# Sparkplug

[![Build Status](https://www.travis-ci.org/freshbooks/sparkplug.svg?branch=master)](https://www.travis-ci.org/freshbooks/sparkplug)
[![PyPi version](https://img.shields.io/pypi/v/sparkplug.svg)](https://pypi.org/project/sparkplug/)

Sparkplug is a lightweight AMQP message consumer. It allows you to specify queue configuration and consumer entry points using INI files

## Testing
run tests with `nosetests`

## Releasing
We release two versions: One to the FreshBooks internal PyPI repository, and one to the public repository.

### Releasing to the FreshBooks internal PyPI repository
Prerequisite: You have an SSH config file with your username, and email located at `~/.gitconfig`. It is needed by the script that bumps the release version.

```VERSION_BUMP_TYPE=minor PYPI_USER=some_user PYPI_PASS=some_password make release```

### Releasing to the public PyPI repository
Once you push a tag, Travis CI builds a new version and pushes it out to public PyPI. There'll be no need to do anything if you just ran the `make release` command from above, to release the library to the FreshBooks internal repository.

## Note

Version 1.11.5, 1.11.6, 1.12.0 are Python 2.7 and 3.x compatible.
Version 1.13.0 and above is not compatible with Python <= 3.4
