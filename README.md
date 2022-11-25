[![test](https://github.com/actions-mn/setup-flavors/actions/workflows/test.yml/badge.svg)](https://github.com/actions-mn/site-gen/actions/workflows/test.yml)

# setup-flavors

Setup extra flavors that aren't come with default `metanorma` installation, like this

```yml
- uses: actions-mn/setup-flavors@main
  with:
    extra-flavors: nist
    github-pakages-token: ${{ secrets.METANORMA_CI_PAT_TOKEN }}
```

Or

```yml
- uses: actions-mn/setup-flavors@main
  with:
    extra-flavors: nist
    github-pakages-token: ${{ secrets.METANORMA_CI_PAT_TOKEN }}
    use-bundler: true
```

> NOTE: this action only works for metanorma from ruby-gems

> NOTE: if `metanorma-cli` installed with `bundle install` make sure to path `use-bundler: true` to the action