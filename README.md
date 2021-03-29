# cloud-object-mappings
A JSON file to store cloud-native objects/resources type and name mappings for multi-flavour cloud providers.

The initiative is to provide a mappings that can be used as a central source to develop multi cloud Infrastcure-as-Code automations.

# Usage

As of now, to query the shortName of AWS containers orchestration service:
```
❯ cat mappings.json | jq '.clouds | .[0].Amazon.compute | .[1].containers.shortName'
"EKS"

```

# References:
https://dzone.com/articles/azure-aws-and-gcp-a-multicloud-service-cheat-sheet
