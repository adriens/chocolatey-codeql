[![Build status](https://ci.appveyor.com/api/projects/status/ydstnokayd3propc?svg=true)](https://ci.appveyor.com/project/adriens/chocolatey-codeql)
[![Chocolatey](https://img.shields.io/chocolatey/v/codeql.svg)](https://chocolatey.org/packages/codeql)
[![Chocolatey](https://img.shields.io/chocolatey/dt/codeql.svg)](https://chocolatey.org/packages/codeql)


# chocolatey-codeql

[Chocolatey](https://chocolatey.org) package source to install [codeql](https://codeql.github.com/docs/codeql-cli/).

# CodeQL CLI

The CodeQL command-line interface (CLI) is used to create databases for security research. You can query CodeQL databases directly from the command line or using the Visual Studio Code extension.

- [Using the CodeQL CLI](https://codeql.github.com/docs/codeql-cli/using-the-codeql-cli/#using-the-codeql-cli) : Software developers and security researchers can secure their code using the CodeQL CLI.
- [CodeQL CLI reference](https://codeql.github.com/docs/codeql-cli/codeql-cli-reference/#codeql-cli-reference): Learn more about the files you can use when running CodeQL processes and the results format and exit codes that CodeQL generates.
- [CodeQL CLI manual](https://codeql.github.com/docs/codeql-cli/manual): Detailed information about all the commands available with the CodeQL CLI.


# Code QL install on Windows

Now, the install process on windows is as easy as :

```
choco install codeql
```

# Prerequisite

Have [chocolatey](https://chocolatey.org/) [properly installed](https://chocolatey.org/install) and web access.


# Install from choco repo

To install schemacrawler, simply run, with ```Administrator``` privileges :

```
choco install codeql
```

Uninstall package :

```
choco uninstall codeql
```




# Build and install commands

With ```Administrator privileges```, run a ```cmd``` shell.

Uninstall package :

```
choco uninstall codeql
```

Manually build and install the package from the source :

```
choco install -fdv codeql.nuspec
```

Push the package to central [package repository](https://chocolatey.org/packages) : check prepared `ant` tasks.

# For developers

For developers, take a look at the ```ant``` build tasks used to automate package compile and build.

Upgrade process:

1. Upgrade verion un properties file
2. `ant make`
3. Install locally `choco install -fdv codeql.nuspec`
4. Test command line `codeql version`
