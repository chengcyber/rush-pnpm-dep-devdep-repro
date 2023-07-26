# Rush pnpm dep devDep issue repro

- rush@5.100.0
- pnpm@8.6.9 (lockfile format v6)

# Steps

```shell
git clone git@github.com:chengcyber/rush-pnpm-dep-devdep-repro.git

cd rush-pnpm-dep-devdep-repro

rush install
```

Outputs

```
The shrinkwrap file contains the following issues:
  Dependencies of project "foo" do not match the current shrinkwrap.


The shrinkwrap file is out of date. You need to run "rush update".
```

Rerunning `rush update` won't solve this issue.
