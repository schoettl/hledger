print-unique\
Print transactions which do not reuse an already-seen description.

_FLAGS_

Example:

```shell
$ cat unique.journal
1/1 test
 (acct:one)  1
2/2 test
 (acct:two)  2
$ LEDGER_FILE=unique.journal hledger print-unique
(-f option not supported)
2015/01/01 test
    (acct:one)             1
```
