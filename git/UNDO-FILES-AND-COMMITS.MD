## UNDO Files and Commits

## Undo files

### If your file is already staged (happens when you do a git add etc after the file is edited) to unstage your changes
```bash
git reset HEAD <file>
git checkout <file>
```

### If not already staged, just use
```bash
git checkout <file>
```
