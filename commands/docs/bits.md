---
title: bits
categories: |
  bits
version: 0.84.0
bits: |
  Various commands for working with bits.
usage: |
  Various commands for working with bits.
---

# <code>{{ $frontmatter.title }}</code> for bits

<div class='command-title'>{{ $frontmatter.bits }}</div>

## Signature

```> bits ```


## Input/output types:

| input   | output |
| ------- | ------ |
| nothing | string |

## Notes
You must use one of the following subcommands. Using this command as-is will only produce this help message.

## Subcommands:

| name                                     | type    | usage                                  |
| ---------------------------------------- | ------- | -------------------------------------- |
| [`bits and`](/commands/docs/bits_and.md) | Builtin | Performs bitwise and for integers.     |
| [`bits not`](/commands/docs/bits_not.md) | Builtin | Performs logical negation on each bit. |
| [`bits or`](/commands/docs/bits_or.md)   | Builtin | Performs bitwise or for integers.      |
| [`bits rol`](/commands/docs/bits_rol.md) | Builtin | Bitwise rotate left for integers.      |
| [`bits ror`](/commands/docs/bits_ror.md) | Builtin | Bitwise rotate right for integers.     |
| [`bits shl`](/commands/docs/bits_shl.md) | Builtin | Bitwise shift left for integers.       |
| [`bits shr`](/commands/docs/bits_shr.md) | Builtin | Bitwise shift right for integers.      |
| [`bits xor`](/commands/docs/bits_xor.md) | Builtin | Performs bitwise xor for integers.     |

**Tips:** Command `bits` was not included in the official binaries by default, you have to build it with `--features=extra` flag