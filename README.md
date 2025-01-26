# AutoHotkey-DecodeUnicodeEscapeSequence
An AutoHotkey (AHK) function that converts all JSON-style Unicode escape sequences within a string to their Unicode characters.

### Example usage
```ahk
Str := ('This function supports characters beyond the Basic Multilingual Plane.'
' Test: These characters: "\u0041\u0042\u0043" should be "ABC".'
' This character: "\uD834\uDD1E" should be a G clef.')
A_Clipboard := DecodeUnicodeEscapeSequence(Str)
; Paste into an editor that supports Unicode supplementary characters. VSCode should support this.
```
