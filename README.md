# python-monorepo

This is my running collections of tools I would use to run a python Monorepo. I
Have used information from lots of sources to put this all together. I will
attempt to link to all of them here:

- https://medium.com/opendoor-labs/our-python-monorepo-d34028f2b6fa
- https://www.tweag.io/blog/2023-04-04-python-monorepo-1/

A lot of this was put together with [@loeken](https://github.com/loeken) whilst
at [@CryptoCompareLTD](https://github.com/CryptoCompareLTD).

# Tools

## Pre-commit hooks

[Pre-commit hooks](https://pre-commit.com/) are a great way to run checks
against the code before it is committed to the repository. This saves time and
money by not having to run checks in the CI/CD pipeline.

It is a python package that can be installed with pip:

```bash
pip install pre-commit
```

Once it is installed you can run the following command to install the hooks:

```bash
pre-commit install
```

Then every time it will run the checks before you commit. If any of the checks
fail it will not allow you to commit. (Though most of the hooks here will sort
the problems out by editing some of the files and telling you what it has
changed.)

You can see what hooks are running in the `.pre-commit-config.yaml` file.
