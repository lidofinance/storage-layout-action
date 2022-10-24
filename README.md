# storage-layout-action

Inspired by https://github.com/odyslam/bash-utils

Simple action to create storage layout file and assert changes in the storage layout after contracts update

## Usage

Generate new .storage-layout file:

```
    steps:
      - uses: lidofinance/storage-layout-action@v1
        with:
          mode: generate
          src-folder: <path to folder with contracts sources>
          ignore-folders: <folder name, or folder names {folder1, folder2, folder3} to exclude>
```

Check new .storage-layout against existing .storage-layout file:

```
    steps:
      - uses: lidofinance/storage-layout-action@v1
        with:
          mode: check
          src-folder: <path to folder with contracts sources>
          ignore-folders: <folder name, or folder names {folder1, folder2, folder3} to exclude>
```
