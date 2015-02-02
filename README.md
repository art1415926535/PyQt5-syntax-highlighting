Python syntax highlighting

If you need a code editor with syntax highlighting, but don't want something as heavyweight as QsciScintilla, you can use the QSyntaxHighlighter class to apply highlighting to a QPlainTextEdit widget. 
This example was based on existing work by Carson Farmer and Christophe Kibleur, and an example on the SciPres wiki. One aspect not addressed by this prior work is handling of Python's triple-quoted strings, which may span multiple lines; the QSyntaxHighlighter documentation includes an example for C++ comments, but those have different beginning and ending delimiters /* ... */, whereas Python's triple-quoted strings have the same delimiter at the beginning and end. These are handled by the match_multiline method--there may be an easier way to do this, but it seems to work pretty well, although it still has trouble with triple-quotes embedded inside another string.

https://wiki.python.org/moin/PyQt/Python%20syntax%20highlighting

UPD: With Darcula theme from PyCharm
