# xsa-db-employees

A simple standalone xsa db repository that contains the following two tables.

|table name| purpose |
|----------|---------|
| person |table for demonstrating extensions in a parent module|
| vacation |just a normal table with association to person|

This micro db module will later be consumed by the companies module.

Since this is a totally standalone db module, this can have a independant application lifecycle of it's own.
All deployments should be patch incremented, so that the parent module can keep using older versions, in case of a backwards
 incompatible change in this child module is made.