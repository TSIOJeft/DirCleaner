# DirCleaner
😘 this is used to store the tasks and config for DirCleaner. and the main purpose is to let gank user to add their custom task and config.
and if something wrong with the task and config you will be appreciated to modify the file by pulling request.😍

## tasks
this folder is the dircleaner task for the formal clean. and the format is below.
```
{
  "Description": "write des here",
  "App": true,
  "Name": "task name",
  "Notice": 0,
  "PackName": "com.pack.com",
  "Paths": [
    "PUBLIC_LOCATION/xxx",
    "PUBLICA_DATA/xxx",
    "PRIVATE_DATA/xxx"
  ],
  "Redirect_Avoid": false,
}
```
`Notice`:

is task notice grade.

0: delete directly

1: delete directly and will show yellow notice in card

2: delete manual and will show red notice in card

`Redirect_Avoid`:

true: redirect app will never effect on the path

false: redirect app will change the path

`Paths`:

is the paths the task will scan.
mutiply path use ',' split.

PUBLIC_LOCATION: will be replace to /storage/emluated/0 by dircleaner

PUBLIC_DATA: will be replace to /storage/emulted/0/Android/data by dircleaner

PRIVATE_DATA: will be replace to /data/data by dircleaner

### How to use task json

`import task`:

enter taskmanage page and press the plus button right top and enter task edit page, long press the save float button the json in your clipboard will be imported.

`export task`:

enter taskmanage page and press the task card you want export will enter task edit page, long press the save float button the json will be copied to your clipboard.

## config
this folder is to store the default config json. and the format is below.

```
{
  "AppClean": {
    "path": [
      "/storage/emulated/0/Android/data/pack/cache",
      "/storage/emluated/0//pack/files/cache",
      "/storage/emulated/0/Android/data/pack/log"
    ],
    "exclude": false
  },
  "ChaosFile": {
    "regex": ".*.(log|logs)",
    "exclude": false
  },
  "ApkClean": {
    "regex": ".*.*(apk|apkm)$",
    "exclude": false
  }
}
```

you can see different block, and it's for `AppClean` `ChaosFile` `ApkClean`.

the AppClean Path is specify the path that appclean should scan and the `pack` in the path will be replace to every app's packname.

the ChaosFile regex is specify the file that which match the regex the file be the chaos file.

the ApkClean regex is specify the file that which match the regex the file be the Apk file.

the `exclude` can not be removed.🤔 However,it's useless.

### How to use the config json

enter setting page and use custom config and paste the config json you copy and save, don't forget restart app.

## pc/program_icons
this folder is for DirCleaner PC version to extend program icon that will show the folder bind with program icon.

## pc/tasks
this folder is for DirCleaner PC version to match the task in the formal clean.
some format will be added later.🤨

# Thanks
that's all, I do hope the task can be more and more that every storage disk junk file can be deleted.

waitting for your PR. 

waitting for your issue.

🤩🤩🤩🤩




