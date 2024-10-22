My goto settings for vscode and related editors setup
# Profiles
| branch   | profile       |
| -------- | ------------- |
| vscode   | flutter       |
# Usage
- install [Sync Settings](https://github.com/zokugun/vscode-sync-settings) extension
- open command palette by pressing `ctrl+shift+p` and open `Sync Settings: Open the repository settings`
- delete everything from file and paste below to sync from this repo:
>>```yml
>>profile: flutter # see below for available profiles
>>
>># sync on remote git
>>repository:
>>  type: git
>>  # url of the remote git repository to sync with, required
>>  url: https://github.com/niamotullah/sync_vscode.git  # https
>>  # url: git@github.com:niamotullah/vscode_sync.git # ssh
>>
>>  # branch to sync on, optional (set to `master` by default)
>>  branch: vscode # see below for available profiles in this branch
>>```
>Learn more about `Sync Settings` extension [here](https://github.com/zokugun/vscode-sync-settings)
- run `Sync Settings: Download (repository -> user)`
- it should ask for necessery github access pass-key if required

To **save** your settings after modification, just run `Sync settings: Upload` from command palette. This will upload modified settings to the repo difined in `url:`




