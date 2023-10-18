# jsdoc-custom-template
Add this jsdoc-config.json file to your js-files directory:

jsdoc-config.json:
```
{
    "tags": {
        "allowUnknownTags": true
    },
    "source": {
        "include": ["apps/js-doc/js-files"] //path to your js-files
    },
    "plugins": ["plugins/markdown"],
    "opts": {
        "encoding": "utf8",
        "template": "node_modules/jsdoc-so-template",
        "destination": "docs/",//index.html file will be generated inside this docs folder
        "recurse": true,
        "verbose": true
    },
    "templates": {
        "cleverLinks": false,
        "monospaceLinks": false,
        "default": {
            "outputSourceFiles": false,
            "includeDate": false,
            "useLongnameInNav": true
        }
    },
    "jsdocSoTemplate": {
        "search": true //enables search in the documentation
    }
}
```
