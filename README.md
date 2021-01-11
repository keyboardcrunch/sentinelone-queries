# SentinelOne Queries
Repository of SentinelOne Deep Visibility queries.

## What These Are
This repository contains yaml files documenting SentinelOne Deep Visibility queries, divided up by Operating System. These yaml files take inspiration from the [SIGMA Signatures](https://github.com/Neo23x0/sigma/) project and provide better programmatic access to SentinelOne queries for the later purpose of mapping to Mitre Attack, providing a query navigator, as well as other hunting tools.

*__Side note:__ Most of these rules were created by converting the markdown files from [ATT&CK Mapped SentinelOne Queries](https://github.com/keyboardcrunch/SentinelOne-ATTACK-Queries) repository. Some of the descriptions, references, and false positive information needs to be cleaned up or filled out.*

## Query Files
Query files document what the goal of the query, references, tags, mitre mapping, and authors. These files can optionally include more than one query, so if you were to create multiple queries for T1055 Process Injection you could store them all in a single file called t1055_process_injection.yml.

```
title:                  -required
description:            -required
author:                 -required
date:                   -optional
modified:               -optional
   tactic:              -optional
   technique:           -optional
   subtechnique:        -optional
operating_system:       -required
query:                  -required
false_positives:        -optional
   - 
tags:                   -optional
   - 
references:             -optional
   -
```

## Work In Progress
This repository is a continuation of the work put forth in the discontinued [SentinelOne ATTACK Queries](https://github.com/keyboardcrunch/SentinelOne-ATTACK-Queries) repository, and as it stands currently, the same Tactic coverage (gaps) exist between both repositories. 
