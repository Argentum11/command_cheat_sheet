# rclone

## mount

```bash
rclone mount REMOTE_NAME: PATH_TO_LOCAL_MOUNT &
disown
```

## stop mounting

```bash
fusermount -u PATH_TO_LOCAL_MOUNT
```

## list trashed files

```bash
rclone lsf REMOTE_NAME: --drive-trashed-only
```

## untrash all files

```bash
rclone backend untrash REMOTE_NAME:
```
