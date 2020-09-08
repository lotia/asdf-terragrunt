# asdf-terragrunt

[![Build Status](https://github.com/lotia/asdf-terragrunt/workflows/CI/badge.svg)](https://github.com/lotia/asdf-terragrunt/actions?query=workflow%3ACI)

Originally from [td7x / asdf / terragrunt on gitlab](https://gitlab.com/td7x/asdf/terragrunt) where it no longer appears to be maintained.

[Terragrunt](https://github.com/gruntwork-io/terragrunt) plugin for the [asdf](https://github.com/asdf-vm/asdf) version manager.
Check out the [asdf](https://github.com/asdf-vm/asdf) readme for instructions.

## Running tests

Some of the binaries have tests. These tests may be executed by setting the
environment variable `ASDF_TERRAGRUNT_TEST=true` when running the program from
the shell.

For example, a successful result looks like this:

```shell
$ ASDF_TERRAGRUNT_TEST=true ./list-all
Running tests ...
Success!
```

Failures will output a diff between the results and expected output:

```diff
$ ASDF_TERRAGRUNT_TEST=true ./list-all
Running tests ...
--- expected
+++ got
@@ -8,4 +8,3 @@
 1.7.0-rc.3
 1.7.0-rc.4
 1.7.0
-1.8.0
Failed!
```
