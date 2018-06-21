autopep8 mirror
=============

Mirror of autopep8 package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For autopep8: see https://github.com/hhatto/autopep8


### Using autopep8 with pre-commit

Add this to your `.pre-commit-config.yaml`:

    -   repo: https://github.com/pre-commit/mirrors-autopep8
        rev: ''  # Use the sha / tag you want to point at
        hooks:
        -   id: autopep8
