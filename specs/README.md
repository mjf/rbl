# RBL Specification YAML Format

```yaml
kind: > #<string>
  | "BlackholeList"
  | "BlackList" # synonym
  | "BlockList" # synonym
  | "WhiteList"
  | "YellowList"
  | "GreyList"
  | "GrayList" # synonym
  | "NoBLList"
  | "ReputationList"
  | "InformativeList"
  | "InformationalList" # synonym
metadata:
  description: #<string>
  name: #<string>
spec:
  queryDomain: #<string>
  type: > #<string>
    | "Domain"
    | "Address"
```

## Example

```yaml
---
kind: BlackList
metadata:
  description: The Spamhaus SBL Advisory
  name: SPAMHAUS-SBL
spec:
  queryZone: sbl.spamhaus.com
```

# RBL Specification Shell Format

## Example

```shell
service
  kind BlackList
  metadata
    description The Spamhaus SBL Advisory
    name SPAMHAUS-SBL
  spec
    queryZone sbl.spamhaus.com
```
