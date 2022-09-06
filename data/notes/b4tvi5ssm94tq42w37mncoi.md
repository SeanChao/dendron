
## Directories

Get parent dir:

from pathlib import Path
path = Path("/here/your/path/file.txt")
print(path.parent.absolute())

mkdir -p: `os.makedirs(xx, exist_ok=True)`
