# [COURSE NAME]
## LAB GUIDES

### AUTHORING NOTES
Enter commands and keystrokes between backticks in MarkDown. 
```
`command -opts ARG1 ARG2`
```
1. `command -opts ARG1 ARG2`
- > Note that commands can be explained with an UL indented blockquote
```
- > UL indented blockquote
```

Keystrokes should be enclosed in backtick quotes AND tagged with angle brackets in commands.
```
`ls<TAB x2>`
```
2. `ls<TAB x2>`

Keystrokes in notes should be made **bold** then backtick enclosed like **`<CTRL+ALT+DEL>`**
```
**`<CTRL+ALT+DEL>`**
```

File paths in notes should be italic like */etc/sudoers*
```
*/etc/sudoers*
```

Text in a file should be opened and closed by 3 backtick quotes like below.

3. Add the following text to the file */etc/sudoers.d/demo*
<pre>
```
instructor  ALL=(ALL)    NOPASSWD:  ALL
```
</pre>

When creating users, groups, shares, etc. make requirements easy to understand with tables.

```
| LEFT_ALIGNED_COL   | CENTERED_COL | RIGHT_ALIGNED_COL |
| :----------------- | :----------: | ----------------: |
| ROW 1 COl 1        | ROW 1 COL 2  | ROW 1 COL 3       |
| ROW 2 COl 1        | ROW 2 COL 2  | ROW 2 COL 3       |
```
The example above looks like this:

| LEFT_ALIGNED_COL   | CENTERED_COL | RIGHT_ALIGNED_COL |
| :----------------- | :----------: | ----------------: |
| ROW 1 COl 1        | ROW 1 COL 2  | ROW 1 COL 3       |
| ROW 2 COl 1        | ROW 2 COL 2  | ROW 2 COL 3       |

******
