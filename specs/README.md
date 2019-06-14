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
