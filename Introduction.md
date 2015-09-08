Fuzzyfinder provides convenient ways to quickly reach the buffer/file you
want. Fuzzyfinder finds matching files/buffers with a fuzzy/partial
pattern to which it converted the entered pattern.

E.g.:
| entered pattern | fuzzy pattern   | partial pattern |
|:----------------|:----------------|:----------------|
| `abc`           | `*a*b*c*`       | `*abc*`         |
| `a?c`           | `*a?c*`         | `*a?c*`         |
| `dir/file`      | `dir/*f*i*l*e*` | `dir/*file*`    |
| `d*r/file`      | `d*r/*f*i*l*e*` | `d*r/*file*`    |
| `../**/s`       | `../**/*s*`     | `../**/*s*`     |

> ( allows searching a directory tree.)

You will be happy when:

  * `"./OhLongLongLongLongLongFile.txt"`
  * `"./AhLongLongLongLongLongName.txt"`
  * `"./AhLongLongLongLongLongFile.txt"` <- you want :O

Type "AF" and `"AhLongLongLongLongLongFile.txt"` will be select. :D


---


Fuzzyfinder has some modes:

  * Buffer mode
  * File mode
  * Directory mode (yet another :cd command)
  * MRU-File mode (most recently used files)
  * MRU-Command mode (most recently used command-lines)
  * Bookmark mode
  * Tag mode (yet another :tag command)
  * Tagged-File mode (files which are included in current tags)


---


Fuzzyfinder supports the multibyte.