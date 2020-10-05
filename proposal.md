## Substring matching

`(string-all-matches `*haystack needle*`)`

Returns a list of indices into *haystack* where *needle* can be found.

`(string-match-fold `*proc knil haystack needle*`)`  
`(string-match-fold-right `*proc knil haystack needle*`)`

Folds over the indices into *haystack* from left to right / right to left
using *proc* and *knil*, and returns the result.

`(string-match-split `*haystack needle*`)`

Returns a list of strings in *haystack* in left to right order that do
not match *needle*

`(string-match-replace `*haystack needle new-needle*`)`  
`(string-match-replace-right `*haystack needle new-needle*`)`  
`(string-match-replace-all `*haystack needle new-needle*`)`

Replaces the first/last/every instance of *needle* in *haystack*
with *new-needle*.

If [SRFI 135](https://github.com/scheme-requests-for-implementation/srfi-135/srfi-135.html),
the above procedures should also be available as `textual-*`.
