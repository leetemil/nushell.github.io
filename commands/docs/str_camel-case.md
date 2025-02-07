---
title: str camel-case
categories: |
  strings
version: 0.84.0
strings: |
  Convert a string to camelCase.
usage: |
  Convert a string to camelCase.
---

# <code>{{ $frontmatter.title }}</code> for strings

<div class='command-title'>{{ $frontmatter.strings }}</div>

## Signature

```> str camel-case ...rest```

## Parameters

 -  `...rest`: For a data structure input, convert strings at the given cell paths


## Input/output types:

| input        | output       |
| ------------ | ------------ |
| list\<string\> | list\<string\> |
| record       | record       |
| string       | string       |
| table        | table        |
## Examples

convert a string to camelCase
```shell
>  'NuShell' | str camel-case
nuShell
```

convert a string to camelCase
```shell
> 'this-is-the-first-case' | str camel-case
thisIsTheFirstCase
```

convert a string to camelCase
```shell
>  'this_is_the_second_case' | str camel-case
thisIsTheSecondCase
```

convert a column from a table to camelCase
```shell
> [[lang, gems]; [nu_test, 100]] | str camel-case lang
╭───┬────────┬──────╮
│ # │  lang  │ gems │
├───┼────────┼──────┤
│ 0 │ nuTest │  100 │
╰───┴────────┴──────╯

```


**Tips:** Command `str camel-case` was not included in the official binaries by default, you have to build it with `--features=extra` flag