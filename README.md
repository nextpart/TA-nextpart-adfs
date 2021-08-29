## AD FS Add-on for Splunk

[![Build Status](https://dev.azure.com/NEXTPART/Splunksters/_apis/build/status/TA-nextpart-adfs?branchName=master)](https://dev.azure.com/NEXTPART/Splunksters/_build/latest?definitionId=61&branchName=master)
[![image](https://img.shields.io/badge/Maintained%20in-Azure%20DevOps-1f425f.svg?logo=Azure%20DevOps)](https://dev.azure.com/NEXTPART/Splunksters)
[![image](https://img.shields.io/badge/Contact-NEXTPART-1abc9c.svg)](mailto:info@nextpart.io)


**ATTENTION**: This is still at an early stage depending on your ADFS servers names containing ADFS.

PRs appreciated!

#### Author information

- Original Author: Nextpart Security Intelligence GmbH
- Version: `X.X.X` (dynamic)
- Date: July 29, 2021

#### Using this Application

- Source: ``XmlWinEventLog:ADFS``
- Sourcetype(s): ``XmlWinEventLog``

###### Upgrade

Remove the app using splunk plugin tool

```
$SPLUNK_HOME/bin/splunk remove app TA-nextpart-adfs
```

###### Install the app

```
 $SPLUNK_HOME/bin/splunk install app <last package file>
```

###### Forwarding Data

Make sure to have the following content in your agents ``inputs.conf``

```toml
[WinEventLog://Security]
disabled = false
whitelist1 = 342,364,4624,4625,4627,4634,4648,4684,1200-1207

[WinEventLog://AD FS/Admin]
disabled = false
whitelist = 342,364
```

#### Update History

- `0.1.X` July 29, 2021: Updates
- `0.0.X` July 29, 2021: Init

#### Copyright & License

Copyright © 2019 Nextpart Security Intelligence GmbH

This program is free software; you can redistribute it and/or modify it under the terms
of the GNU General Public License as published by the Free Software Foundation; either
version 2 of the License, or (at your option) any later version.

Find more information about this on the [LICENSE](./LICENSE) file.

