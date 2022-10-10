# indesign-grep-scripting
These patterns applies to Spanish language.
All these patterns have false positives, which means that they requires a manual case by case evaluation. 

###Pattern <word><puntuation><word>
```
[\l\u][,\.:;][\l\u]
```
False positive: urls and acronyms.

### Space before opening sign ( ¿ [ « “
```
[\(“«\¿\[]\s
```
False positives: quotes in french.

### Space before closing sign
```
\s[,\.:;\)\]\?”»]
``` 
False positives: quotes in french.

### Space, comma or punctuation before "call-to-note" sign
´´´
[\s,\.:;]~F
```
False positives: none, unless the text is in English.


\([^\)]+\(
«[^»]+«
.
‘[^’]+‘
\¿[^\?]+\¿

[^\.^;^:^\?^…^S]$

\>\s[;,;\.]




,,

Palabras que se repiten: \b(\w+) +\1\b

~S$

”,
