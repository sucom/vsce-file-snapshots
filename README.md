# VS Code Extension: File Snapshots

Never lose your progress — instantly back up your file before every edit, whether by you or your AI.

To backup a folder, checkout [Backup Folder](https://marketplace.visualstudio.com/items?itemName=spajs.backup-folder) extension.

## Installation

- Install from [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=spajs.backup-file)

- Command Line: `code --install-extension spajs.backup-file`

OR

1. Open VS Code
2. Go to Extensions
3. Search "Backup File"
4. Click **Install**

## Usage

#### Using editor toolbar buttons

- *Location*: Top-right corner of active editor
- *Visible* only when file is opened and focused
- *Icons*: 💾=save | refresh=restore last snapshot

#### Using status bar buttons

- 🧹: Clear old snapshots

#### Keyboard shortcuts

- [ ctrl + shift + b ] : Backup
- [ ctrl + shift + r ] : Restore last snapshot


## Configuration

### Extension Settings (Ctrl + ,)

`File` → `Preferences` → `Settings` → Search "backupFile"

```backupFile.backupDirectory```: Custom backup directory path. If empty, defaults to .vscode/file-snapshots in the current workspace.

```backupFile.autoBackupOnSave```: Automatically backup files when they are saved.

```backupFile.backupOnlyOnDiff```: If enabled, creates backup only on content diff or ignores. If disabled, creates backup on request.

```backupFile.preserveFolderStructure```: Preserve the original folder structure in backups.

```backupFile.cleanupDays```: Number of days to keep backup files before they can be cleaned up.

```backupFile.autoCleanup```: Automatically clean up old backup files when creating new backups.

## License

MIT

## Home

[Git](https://github.com/sucom/vsce-backup-file)
