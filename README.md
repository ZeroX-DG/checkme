checkme
=======

A simple todo cli app build with oclif

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/checkme.svg)](https://npmjs.org/package/checkme)
[![CircleCI](https://circleci.com/gh/ZeroX-DG/checkme/tree/master.svg?style=shield)](https://circleci.com/gh/ZeroX-DG/checkme/tree/master)
[![Appveyor CI](https://ci.appveyor.com/api/projects/status/github/ZeroX-DG/checkme?branch=master&svg=true)](https://ci.appveyor.com/project/ZeroX-DG/checkme/branch/master)
[![Codecov](https://codecov.io/gh/ZeroX-DG/checkme/branch/master/graph/badge.svg)](https://codecov.io/gh/ZeroX-DG/checkme)
[![Downloads/week](https://img.shields.io/npm/dw/checkme.svg)](https://npmjs.org/package/checkme)
[![License](https://img.shields.io/npm/l/checkme.svg)](https://github.com/ZeroX-DG/checkme/blob/master/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g checkme
$ checkme COMMAND
running command...
$ checkme (-v|--version|version)
checkme/1.0.0 linux-x64 node-v8.9.4
$ checkme --help [COMMAND]
USAGE
  $ checkme COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`checkme add [TODO]`](#checkme-add-todo)
* [`checkme remove [TODO]`](#checkme-remove-todo)
* [`checkme list`](#checkme-list)
* [`checkme interact`](#checkme-interact)
* [`checkme help [COMMAND]`](#checkme-help-command)

## `checkme add [TODO]`

Add new todo to list

```
USAGE
  $ checkme add [TODO]

OPTIONS
  -d, --done  mark todo as done

EXAMPLES

  $ checkme add "a new todo"
  [Success] Added new todo: a new todo


  $ checkme add
  ›   Error: please specify the new todo
```

_See code: [src/commands/add.ts](https://github.com/ZeroX-DG/checkme/blob/v1.0.0/src/commands/add.ts)_

## `checkme remove [TODO]`

Remove a todo from list

```
USAGE
  $ checkme remove [INDEX]

EXAMPLES

  $ checkme remove 0
  [Success] Removed todo: a new todo


  $ checkme remove
  ›   Error: please specify the todo's index
```

_See code: [src/commands/remove.ts](https://github.com/ZeroX-DG/checkme/blob/v1.0.0/src/commands/remove.ts)_

## `checkme list`

Print out all todos

```
USAGE
  $ checkme list
```

_See code: [src/commands/list.ts](https://github.com/ZeroX-DG/checkme/blob/v1.0.0/src/commands/list.ts)_

## `checkme interact`

Enter the interacting mode

```
USAGE
  $ checkme interact
```

_See code: [src/commands/interact.ts](https://github.com/ZeroX-DG/checkme/blob/v1.0.0/src/commands/interact.ts)_

## `checkme help [COMMAND]`

display help for checkme

```
USAGE
  $ checkme help [COMMAND]

ARGUMENTS
  COMMAND  command to show help for

OPTIONS
  --all  see all commands in CLI
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v2.0.5/src/commands/help.ts)_
<!-- commandsstop -->
