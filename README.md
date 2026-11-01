# scoop-bucket

Scoop bucket for [shipsmoke](https://github.com/geyutu6755/shipsmoke) —
verify that release artifacts (zip, tar.gz, binaries) actually extract and
run on the target OS.

```powershell
scoop bucket add geyutu6755 https://github.com/geyutu6755/scoop-bucket
scoop install shipsmoke
shipsmoke version
```

The manifest is updated with every shipsmoke release; an Actions workflow in
this repository installs it with Scoop on a Windows runner and runs the
built-in check on every push.
