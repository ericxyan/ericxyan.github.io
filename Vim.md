# Vim
## **find and replace**
- searching: ``:s/string``
- replacing: ``:s/\<pattern\>/replace/gci``
    - ``g`` - all lines
    - ``c`` - ask for confirmation
    - ``i`` - case insnesitive, ``I`` - sensitive
    - ``\<pattern\>`` - the whole word exactly matching ``pattern``
    - ``:s/`` - in the current line
    - ``:%s/`` - all lines
    - ``:5,12s/`` - line 5 to line 12 (inclusive)
    - ``:.,$s/`` - current line to the last line
    - ``:.,+2s/`` - current line to the two next lines
    - ``:g/

