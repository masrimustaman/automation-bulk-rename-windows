## To append prefix to all files under current folder
```
$files = ls
foreach ($s in $files.name){$newname = "DCCTSTVCENTER_" + $s; Move-Item $s -Destination $newname}
```


## To rename prefix to all files under current folder
```
$files = ls
foreach ($s in $files.name){$newname = $s -replace "RCAPVMCENTER", "RCAPVMCENTER_"; Move-Item $s -Destination $newname}
```
