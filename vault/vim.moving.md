---
id: WAZDIhNBmlbDYYcAW85dK
title: Moving
desc: ''
updated: 1647842337586
created: 1629257563529
---

## Moving around

```text
                        +---------------------------+
                H -->   | text sample text          |
                        | sample text               |
                        | text sample text          |
                        | sample text               |
                M -->   | text sample text          |
                        | sample text               |
                        | text sample text          |
                        | sample text               |
                L -->   | text sample text          |
                        +---------------------------+
```

### Scrolling

```text
                                       +----------------+
                                       | some text      |
                                       | some text      |
                                       | some text      |
        +---------------+              | some text      |
        | some text     |  CTRL-U  --> |                |
        |               |              | 123456         |
        | 123456        |              +----------------+
        | 7890          |
        |               |              +----------------+
        | example       |  CTRL-D -->  | 7890           |
        +---------------+              |                |
                                       | example        |
                                       | example        |
                                       | example        |
                                       | example        |
                                       +----------------+

zz: focus on current line
```

## Marks and Jump

`` ` ` ``, `''`: [JUMP] jump back (to exact column, beginning of line)

`CTRL-O`: jumps to older positions

`CTRL-I`: jumps to newer positions

`ms`: mark current position to s

`` `s``, `'s`: jump to mark s

        '       The cursor position before doing a jump
        "       The cursor position when last editing the file
        [       Start of the last change
        ]       End of the last change
