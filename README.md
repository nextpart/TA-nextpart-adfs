
# TEMPLATE Application/Add-on for Splunk

[![Build Status](https://dev.azure.com/NEXTPART/Splunksters/_apis/build/status/TEMPLATE?branchName=master)](https://dev.azure.com/NEXTPART/Splunksters/_build/latest?definitionId=55&branchName=master) [![image](https://img.shields.io/badge/Maintained%20in-Azure%20DevOps-1f425f.svg?logo=Azure%20DevOps)](https://dev.azure.com/NEXTPART/Splunksters) [![image](https://img.shields.io/badge/Contact-NEXTPART-1abc9c.svg)](mailto:info@nextpart.io)

## Author information

- Original Author: Nextpart Security Intelligence GmbH
- Version: ``X.X.X`` (dynamic)
- Date: July 29, 2020

## Using this Application

Source: ``<SOURCE>``
Sourcetype: ``<SOURCETYPE>``

### Upgrade
Remove the app using splunk plugin tool

```
$SPLUNK_HOME/bin/splunk remove app <TEMPLATE>
```

### Install the app


```
 $SPLUNK_HOME/bin/splunk install app <last package file>
```

### Forwarding Data


## Update History

* ``0.0.0`` July 29, 2020:
    Init


## Copyright & License

Copyright © 2019 Nextpart Security Intelligence GmbH

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

Find more information about this on the [LICENSE](./LICENSE) file.