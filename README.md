![build-test](https://github.com/jkroepke/setup-helmfile/workflows/build-test/badge.svg)

## Setup helmfile ##
GitHub Action for installing [variantdev/helmfile](https://github.com/variantdev/helmfile)

#### Repurposed from [mdgreenwald/mozilla-sops-action](https://github.com/mdgreenwald/mozilla-sops-action) ####

Install a specific version of helmfile binary on the runner.
Acceptable values are latest or any semantic version string like v2.16.7 Use this action in workflow to define which version of helmfile will be used.

```yaml
- uses: jkroepke/setup-helmfile@v1
  with:
    version: '<version>' # default is latest stable
  id: install
```

The cached helmfile binary path is prepended to the PATH environment variable as well as stored in the helmfile-path output variable. Refer to the action metadata file for details about all the inputs [here](https://github.com/jkroepke/setup-helmfile/blob/master/action.yml).
