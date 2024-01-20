# JSON first

- Create a file called `Database.json` inside the root directory of your module
- Valid properties are:
    - `name` (required)
    - `tables` (optional)
    - `views` (optional)
- To generate code and database, `Setup` an API project, for example `AdminApi` or `SiteApi`
- `Enter`
- `Generate ModuleName`

A sample of a `Database.json` for a simple blog:

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
hasGuid
hasImage
hasKey
hasOrder
hasSlug
hasTitle
hasVital
