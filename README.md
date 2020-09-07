# rfcbib
A BibTeX file at almost all RFCs.

## Regular Expressions

`RFC([0-9]{1,4}) (.+?)\. (.+)\. ([0-9]{1,2} )?(January|February|March|April|May|June|July|August|September|October|November|December) ([0-9]{4})\. .+`

`@techreport{RFC$1,\n  url = {https://www.rfc-editor.org/rfc/rfc$1.txt},\n  author = {$3},\n  title = {$2},\n  howpublished = {Internet Requests for Comments},\n  type = {RFC},\n  number = {$1},\n  year = {$6},\n  month = {$5},\n  issn = {2070-1721},\n  publisher = {RFC Editor},\n  institution = {RFC Editor},\n}`

---

`\{RFC([0-9]{1}),`

`{RFC000$1,`

---

`\{RFC([0-9]{2}),`

`{RFC00$1,`

---

`\{RFC([0-9]{3}),`

`{RFC0$1,`

---

`^(?=  author)(.*)(, )(.*)`

`$1 and $3`
