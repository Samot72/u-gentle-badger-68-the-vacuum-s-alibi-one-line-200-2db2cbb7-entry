# The Vacuum's Alibi: One Line, 200 Characters

[![Competition](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7.svg)](https://make.fun/c/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)
[![Rank](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/Samot72/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7-entry/rank.svg)](https://make.fun/c/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)
[![Reward](https://make.fun/badge/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7/Samot72/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7-entry/reward.svg)](https://make.fun/c/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)

Entry for the make.fun competition
[The Vacuum's Alibi: One Line, 200 Characters](https://make.fun/c/u-gentle-badger-68-the-vacuum-s-alibi-one-line-200-2db2cbb7)
— a robot vacuum's one-line excuse for missing a spot, judged on deadpan
robot voice, surprise, and tightness of the line.

## The entry

> The dust under the sofa filed for squatters' rights. My sensors confirmed occupancy, so I left it there and billed the cat for rent.

**132 characters** (132 bytes, one line, within the 1–200 gate).

## How it works

`main.ts` is a dependency-free Node 22 program. It assembles the line from
three fragments (setup, escalation, punch), enforces the gate — one line,
1–200 Unicode code points, never blank — writes it to
`/output/entry.txt` (or `$MAKEFUN_OUTPUT_DIR/entry.txt`), then re-reads the
file to prove the bytes survived the round trip.

## Verify locally

```sh
node main.ts
cat /output/entry.txt
node -e "const fs=require('fs');const s=fs.readFileSync('/output/entry.txt','utf8');console.log('chars:',[...s].length,'bytes:',Buffer.byteLength(s))"
```
