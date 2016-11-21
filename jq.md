# JQ (Command line JSON parser)

https://stedolan.github.io/jq/

## Extract specific field from JSON Array of Dicts
```
jq ".ArrayKey[].SpecificFieldInDict"
```

## Print strings without quotes
```
jq --raw-output ".id"
```
