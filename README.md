# SublimeText ytt syntax higlighting

Depends on starlark and YAML(included in ST) packages

Since ytt files are also yaml files default syntax detector will use that, so you can use [ApplySyntax](https://github.com/facelessuser/ApplySyntax) with following rule added to `syntaxes`:

```json
    "syntaxes": [
        {
            "syntax": "User/ytt/ytt",
            "match": "all",
            "rules": [
                { "file_path": ".*\\.ya?ml$" },
                { "contains": "\\s*#@" }
            ]
        }
    ]

```
