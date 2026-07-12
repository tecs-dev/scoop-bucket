# tecs-dev Scoop Bucket

Scoop manifests for [Tecs](https://github.com/tecs-dev/tecs) tooling.

## Install

```powershell
scoop bucket add tecs https://github.com/tecs-dev/scoop-bucket
scoop install tecs
```

Then create your first project:

```powershell
tecs new hello
cd hello
tecs run
```

The first `tecs` command downloads the LÖVE 12 runtime into your user cache;
later commands reuse it. No Lua, LuaRocks, or compiler toolchain is required.

## Updates

The Excavator workflow polls
[tecs-cli releases](https://github.com/tecs-dev/tecs-cli/releases) and rewrites
the manifest to each new release's `tecs-cli-<version>-windows.zip`, verifying
hashes against the published `SHA256SUMS`.
