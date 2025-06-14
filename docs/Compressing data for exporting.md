---
author: Aliafriend/Chris Carpenter
tags:
  - advice
  - technique
---
https://docs.google.com/spreadsheets/d/1FHIZ6dhf4LYMnqH460OgUB002Paww7YXXkYzGMweMzE/\

Sometimes we have too many cells for things like IMPORTRANGE() or IMPORTRANGE() takes awhile to load slowing down our sheet. We can use this method of compressing the data to speed things up or bypass cell limits.

Packing the data we will use typically un-used characters such as | and ~ to join each column into a single string, from there we join all of the columns to create a single string that will be our import cell (or import string if you're doing it manually.

`=LAMBDA(columns,JOIN("~",BYCOL(columns,lambda(col,JOIN("|",col)))))(columns)`

Unpacking the data we will just split in the reverse order that we packed it putting the data in it's original locations therefore bypassing cell limits. It will also increase the speed of the import/export because it's only looking at a single cell for data.

`=LAMBDA(packed_data,MAP(SPLIT(packed_data,"~"),lambda(a,tocol(SPLIT(a,"|")))))(packed_data)`