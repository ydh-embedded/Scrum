
#powershell 

_____________

`(base) PS C:\working-directory\MindMappping\root-Obsidian> `
```bash
	Get-ChildItem -Filter "Pasted-image-*.png" | ForEach-Object {
    $newName = "Obsidian-" + $_.Name.Split('-')[-1]
    Copy-Item -Path $_.FullName -Destination $newName
	}
```
``(base) PS C:\working-directory\MindMappping\root-Obsidian>``
.

