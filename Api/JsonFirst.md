# JSON first

- Create a file called `Part.json` inside the API directory of your module
- Valid properties are:
    - `name` (required)
    - `tables` (optional)
- To generate code and database, `Setup` an API project, for example `AdminApi` or `SiteApi`
- `Enter`
- `Generate ModuleName`

A sample of a `Part.json` for a simple blog:

```
{
    "name": "Blog",
    "tables": [
        {
            "name": "Posts",
            "columns": [
                {
                    "name": "Title"
                }
            ]
        }
    ]
}
```

hasContent
hasDefault
hasEntityType
hasUuid
hasImage
hasKey
hasOrder
hasSlug
hasTitle
hasVital
