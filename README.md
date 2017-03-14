To reproduce the error, run `tsc` at the root of this project.

Tested with versions:
  * 2.2.1
  * 2.2.2-insiders.20170302
  * 2.3.0-dev.20170314

Expected output:

```
$ tsc

2   export enum Enum {One=1}
                      ~~~

node_modules/@types/foo/index.d.ts(2,21): error TS2300: Duplicate identifier 'One'.


2   export enum Enum {One=1}
                      ~~~

node_modules/bar/node_modules/@types/foo/index.d.ts(2,21): error TS2300: Duplicate identifier 'One'.

```
