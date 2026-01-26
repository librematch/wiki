# Localization

To have our responses in different languages, we want to use [Project Fluent (Python)](https://github.com/projectfluent/python-fluent/tree/master/fluent.runtime#fluentruntime-) as a framework in the backend.

This would imply, that we convert the official translations into `ftl` files.

```bash
l10n/
  de/
    main.ftl
  en-US/
    main.ftl
```

The conversion could be done in the [Collector](../collector/) and then our [Persistence Controller](../persistence/) writes the data to our file system.
For reading, writing and transforming Fluent files, there is the [Fluent Syntax](https://github.com/projectfluent/python-fluent/tree/master/fluent.syntax) library.

[Python Fluent](https://github.com/projectfluent/python-fluent) code would look like this:

```python
# initialize the loader with the locales
from fluent.runtime import FluentLocalization, FluentResourceLoader
loader = FluentResourceLoader("l10n/{locale}")

# we would pull all localisations in here and have one huge object in memory
l10n = FluentLocalization(["de", "en-US"], ["main.ftl"], loader) 

# then we can query our localisations like this
val = l10n.format_value("my-first-string")
"Fluent can be easy"
```

## Advantages

- contributions to localisation made easy
- extra effort, due to versioning in another repository
- has implementations for different programming languages

1. [JavaScript](https://github.com/projectfluent/fluent.js)
1. [Python](https://github.com/projectfluent/python-fluent)
1. [Rust](https://github.com/projectfluent/fluent-rs)

## Disadvantages

- file system storage
- probably versioning in another repository needed
- another dependency
