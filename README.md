# OpenClaw Backups

This repository stores chunked OpenClaw backup artifacts for GitHub-compatible pushes.

## Restore a backup

1. Enter the desired artifact directory under `artifacts/<timestamp>/`
2. Reassemble the archive:

```bash
cat openclaw-*.tar.gz.part-* > openclaw-restore.tar.gz
```

3. Verify checksum using `latest-backup.json`
4. Extract with:

```bash
tar -xzf openclaw-restore.tar.gz -C ~
```
