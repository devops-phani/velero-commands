# velero-commands

### Create backup from schedule

```
velero backup create --from-schedule my-backup
```

### Restore the backup and exclude pv

```
velero restore create my-restore --from-backup my-backup-20240729201518 --exclude-resources pv
```

### Restore backup to different namespace

```
velero restore create my-restore --from-backup my-backup-20240729201518 --namespace-mappings mynamespace:test
```
