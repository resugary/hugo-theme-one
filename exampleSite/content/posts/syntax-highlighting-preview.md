---
title: "Syntax Highlighting Preview"
date: 2017-12-20T12:33:21+08:00
tags: ["example","code"]
draft: false
---

Hugo comes with really fast syntax highlighting from Chroma and provides a [Chroma style gallery](https://xyproto.github.io/splash/docs/all.html). You can configure syntax highlighter in the `config.toml` file. The theme one uses the pygments style color style. 

CSS

```css
@font-face {
  font-family: Chunkfive; src: url('Chunkfive.otf');
}

body, .usertext {
  color: #F0F0F0; background: #600;
  font-family: Chunkfive, sans;
}

@import url(print.css);
@media print {
  a[href^=http]::after {
    content: attr(href)
  }
}
```

JavaScript

```javascript
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1)
      return process(block, true, 0x0F) +
             ` class="${cls}"`;
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i < classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }
}

export  $initHighlight;
```

Python

```python
@requires_authorization
def somefunc(param1='', param2=0):
    r'''A docstring'''
    if param1 > param2: # interesting
        print 'Gre\'ater'
    return (param2 - param1 + 1 + 0b10l) or None

class SomeClass:
    pass

>>> message = '''interpreter
... prompt'''
```

Shell Session

```shell
$ echo $EDITOR
vim
$ git checkout master
Switched to branch 'master'
Your branch is up-to-date with 'origin/master'.
$ git push
Everything up-to-date
$ echo 'All
> done!'
All
done!
```

