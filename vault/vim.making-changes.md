---
id: shmxo9dIs6YlQNYdfI41a
title: Making Changes
desc: ''
updated: 1629339766933
created: 1629264231044
---

🔗 [vimhelp](https://vimhelp.org/usr_04.txt.html)

## Common

        X  stands for  dh  (delete character left of the cursor)
        D  stands for  d$  (delete to end of the line)
        C  stands for  c$  (change to end of the line)
        s  stands for  cl  (change one character)
        S  stands for  cc  (change a whole line)

## Clipboard

To copy a line to the clipboard:

        "*yy

To put text from the clipboard back into the text:

        "*p

## Text Objects

        diw     delete a word (excluding right white space)
        daw     delete a word (including right white space)
        cis     change inner sentence
