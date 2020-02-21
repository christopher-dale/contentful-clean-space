contentful-clean-space
======================
CLI toop to delete all content entries from a specified environment. This fork removes any places where the environment is defaulted to 'master' and makes `env` a required option.

[Contentful CLI](https://github.com/contentful/contentful-cli) doesn't have a command to delete all entries from a space without deleting the space itself. However, this can be very useful, e.g. for user contract testing.

Installation
------------
Using npm:
```
npm install -g contentful-clean-space
```

Usage
-----
```
contentful-clean-space
Options:
  --help           Show help                                           [boolean]
  --space-id       Contentful space id                       [string] [required]
  --env            Contentful environment                    [string] [required]
  --accesstoken    Contentful access token                   [string] [required]
  --batch-size     Number of parallel contentful requests  [number] [default: 5]
  --content-types  Delete content types as well       [boolean] [default: false]
  --yes, -y        Auto-confirm delete prompt         [boolean] [default: false]
  --verbose, -v                                       [boolean] [default: false]
```
All parameters can be provided from environment variables, too. To do that, just set an environment variable using UPPER_CASE casing.
