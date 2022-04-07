---
id: b4tvi5ssm94tq42w37mncoi
title: Fs
desc: ''
updated: 1649146598867
created: 1649146598867
---

## Directories

Get parent dir:

from pathlib import Path
path = Path("/here/your/path/file.txt")
print(path.parent.absolute())

mkdir -p: `os.makedirs(xx, exist_ok=True)`
