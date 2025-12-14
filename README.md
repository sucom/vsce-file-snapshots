# VS Code Extension: File Snapshots

Never lose your progress — instantly back up your file before every edit, whether by you or your AI.

To backup a folder, checkout [Backup Folder](https://marketplace.visualstudio.com/items?itemName=spajs.backup-folder) extension.

## Installation

### Recommended

1. Open VS Code
2. Go to Extensions
3. Search "File Snapshots"
4. Click **Install**

### Alternative Methods

- Install from [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=spajs.file-snapshots)

- Command Line: `code --install-extension spajs.file-snapshots`

## Usage

#### Using editor toolbar buttons

- *Location*: Top-right corner of active editor
- *Visible* only when file is opened and focused
- *Icons*: 💾=save | refresh=restore last snapshot/backup

#### Using status bar buttons

- 🧹: Clear old snapshots

#### Keyboard shortcuts

- [ ctrl + shift + b ] : Backup
- [ ctrl + shift + r ] : Restore last snapshot


## Configuration

### Extension Settings (Ctrl + ,)

`File` → `Preferences` → `Settings` → Search "fileSnapshots"

```fileSnapshots.backupDirectory```: Custom backup directory path. If empty, defaults to .vscode/file-snapshots in the current workspace.

```fileSnapshots.autoBackupOnSave```: Automatically backup files when they are saved.

```fileSnapshots.backupOnlyOnDiff```: If enabled, creates backup only on content diff or ignores. If disabled, creates backup on request.

```fileSnapshots.preserveFolderStructure```: Preserve the original folder structure in backups.

```fileSnapshots.cleanupDays```: Number of days to keep backup files before they can be cleaned up.

```fileSnapshots.autoCleanup```: Automatically clean up old backup files when creating new backups.

## License

MIT
