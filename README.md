# libra
A shell library for collecting, tagging your favorite reading materials.

## Architecture
`librad` keeps running as backend server which takes responsibilities for managing all the materails and its tag indexing.

`libra` is an front-end command tool taking responsibilities for interacting with `librad` server.

And you should understand such architecture is suitable for deploying a remote `librad`.

## Command 
### add
`add` should support adding a material from a path or url(http only now) and of course multiple tags can be assigned when adding.

### tag
Any material can be assigned multiple tags which can be used to provide indexing when you want to search some kind of materials so `tag` command is used to manage all the tags.

### list
`list` command should support listing materials (with limit and specific order) or some ones filtering by some tags.

### open
`open` command can be used to open a materail with right program which should be decided by a config.

### delete
`delete` command can be used to remove material to trash or remove materail totally.

### trash
`trash` command can be used to recovery/empty trash.
