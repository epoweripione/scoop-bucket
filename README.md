# Personal collection bucket for [Scoop](http://scoop.sh)

To make it easier to install apps from this bucket, run:

`scoop bucket add epower https://github.com/epoweripione/scoop-bucket`

# [App Manifest Autoupdate Workflow](https://github.com/lukesampson/scoop/wiki/App-Manifest-Autoupdate)

```
cd <bucket repository>
# .\bin\checkver.ps1 -App chromium-official-dev -Update
.\bin\checkver * -u # updates all manifest in the repo
git commit -m "Updated apps"
git push
scoop update
scoop status
scoop update <app>
```