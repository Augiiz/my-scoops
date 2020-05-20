# for gcc 10

scoop bucket add versions

scoop install 7zip-zstd

scoop uninstall 7zip

* Add zst to Line 19 of lib/decompress.ps1 of scoop (%SCOOP%/apps/scoop/current/lib/decompress.ps1) example of line below:

> return $File -match '\.((gz)|(tar)|(tgz)|(lzma)|(bz)|(bz2)|(7z)|(rar)|(iso)|(xz)|(lzh)|(nupkg)|(zst))$'

scoop reset 7zip-zstd
