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

## Make each JSON object only take up 1 line
```
# Quickly count how many objects there are
jq ".events[].message" --compact-output | wc -l
```

## Get a range of a JSON array
```
jq ".events[0:6]"
```
