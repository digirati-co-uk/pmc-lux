# Roles

The key is the string extracted from the `<persauthorfull>` element. For example:

```
<persauthorfull>Jarman, Derek [1942-1994.] (author)</persauthorfull>
```

The string "author" is extracted from this record, and is used as a key in roles.json to find:

```json
{
    "_activity": "Production",
    "id": "http://vocab.getty.edu/aat/300025492",
    "type": "Type",
    "_label": "author"
}
```

The `_activity` field is used to provide the `type` of Activity this is when applied to a bibliographic record (Production, Creation etc).

Here the `_label` is usually the same as the key but this might not be desired.

`_note` is only used in this JSON and is not carried into the transformed data.


