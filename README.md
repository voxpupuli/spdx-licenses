# spdx-licenses

A Ruby library around the [SPDX license data](http://spdx.org/licenses/),
which provides a set of standard identifiers for open source licenses.

The data is maintained by [SPDX](http://spdx.org/). This library
redistributes the [licenses JSON file](https://spdx.org/licenses/licenses.json).

## Installation

    $ gem install spdx-licenses

or in your Gemfile:

    gem 'spdx-licenses'

## Versioning

This gem and its API is versioned according to semver.  Minor releases may
contain updates to the SPDX License List data.

| spdx-licenses | SPDX License List |
|---------------|-------------------|
| 1.0.0         | 1.2.0             |
| 1.1.0         | 2.4               |
| 1.2.0         | 3.1               |
| 1.3.0         | 3.11-54           |
| 1.4.0         | 3.27.0            |

## Usage

    > lic = SpdxLicenses.lookup('Apache-2.0')
    > lic.id
    "Apache-2.0"
    > lic.name
    "Apache License 2.0"
    > lic.osi_approved?
    true
    > SpdxLicenses.lookup('Unknown')
    nil

    > SpdxLicenses.exist?('Apache-2.0')
    true
    > SpdxLicenses.exist?('Unknown')
    false

## Transfer notice

Version 1.3.0 and older were maintained by Dominic Cleal.
Aftwards the project got migrated to Vox Pupuli.

## License

Copyright (c) 2014-2021 Dominic Cleal.  Distributed under the MIT license.
