## To append prefix to all files under current folder
```
$files = ls
foreach ($s in $files.name){$newname = "prefix01_" + $s; Move-Item $s -Destination $newname}
```


## To rename prefix to all files under current folder
```
$files = ls
foreach ($s in $files.name){$newname = $s -replace "prefix01_", "prefix02_"; Move-Item $s -Destination $newname}
```
