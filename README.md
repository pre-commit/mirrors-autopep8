autopep8 mirror
===============

Mirror of autopep8 package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For autopep8: see https://github.com/hhatto/autopep8


### Using autopep8 with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
-   repo: https://github.com/pre-commit/mirrors-autopep8
    rev: ''  # Use the sha / tag you want to point at
    hooks:
    -   id: autopep8
```

### overriding `args`

note that [this repository] sets `args: [-i]`, if you are configuring autopep8
using `args` you'll want to include either `-i` (`--in-place`) or
`-d` (`--diff`).  it is usually better to configure `autopep8` in its
[config file].

[this repository]: https://github.com/pre-commit/mirrors-autopep8/blob/5c459f3f27ae62fefef60fe5771e51baa02e7a83/.pre-commit-hooks.yaml#L6
[config file]: https://github.com/hhatto/autopep8#configuration
