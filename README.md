# Learn Regex
Examples based regex learning

## Character Handling
### basic match
Matches exact characters.

<pre>
man => The <a href="#x">man</a> and wo<a href="#x">man</a>.
</pre>


### [abc] character set
Matches any character in the set.

<pre>
[tT]he => <a href="#x">The</a> man and <a href="#x">the</a> woman.
[bc]at => The <a href="#x">cat</a> and the <a href="#x">bat</a> and the rat are having a chat.
</pre>

### [^abc] negated set
Matches any character that is not in the set.

<pre>
[^bc]at => The cat and the bat and the <a href="#x">rat</a> are having a c<a href="#x">hat</a>.
</pre>

### [a-z] range set
Matches any character between the the two specified character.

<pre>
[0-9] => My ID number is <a href="#x">176584</a>.
</pre>

### . dot operator
Matches any character except linebreaks.

<pre>
.at => The <a href="#x">cat</a> and the <a href="#x">bat</a> and the <a href="#x">rat</a> are having a c<a href="#x">hat</a>.
</pre>

Equivalent: [^\n\r]

### \w word
Matches any word (alphanumeric and underscore).

<pre>
\w => <a href="#x">PI</a> (π) = <a href="#x">3</a>.<a href="#x">1416</a>
</pre>

Equivalent: [a-zA-Z0-9_]

### \W not word
Matches any non word (not alphanumeric and underscore).

<pre>
\W => PI<a href="#x"> π = </a>3<a href="#x">.</a>1416</a>
</pre>

Equivalent: [^a-zA-Z0-9_]

### \d digit
Matches any digit.

<pre>
\d => PI (π) = <a href="#x">3</a>.<a href="#x">1416</a>
</pre>

Equivalent: [0-9]

### \D not digit
Matches any non digit.

<pre>
\D => <a href="#x">PI (π) = </a>3<a href="#x">.</a>1416
</pre>

Equivalent: [^0-9]

### \s whitespace
Matches any whitespace.

<pre>
\s => PI<a href="#x"> </a>(π)<a href="#x"> </a>=<a href="#x"> </a>3.1416
</pre>

### \S whitespace
Matches any non whitespace.

<pre>
\S => <a href="#x">PI</a> <a href="#x">(π)</a> <a href="#x">=</a> <a href="#x">3.1416</a>
</pre>


## Anchors
### ^ beginning
Matches at the beginning.

<pre>
^P[iI] => <a href="#x">PI</a> (π) = 3.1416
</pre>

Don't be confused with `[^iT]` that means not any of i and I.

### $ end
Matches at the end.

<pre>
\d$ => PI (π) = 3.141<a href="#x">6</a>
</pre>

### \b word boundary
Matches at the end of each word.

<pre>
an\b => The m<a href="#x">an</a> and wom<a href="#x">an</a>.
</pre>

### \B not word boundary
Matches not at the end of each word.

<pre>
an\B => The man <a href="#x">an</a>d woman.
</pre>


## Escaped characters
### \ reserved character
Matches special reserved characters `+*?^$\.[]{}()|/`.

<pre>
\(\S\) => PI <a href="#x">(π)</a> = 3.1416
</pre>

### \t tab
Matches a TAB character.

<pre>
\t => Tab1<a href="#x">	</a>Tab2
</pre>


### others
<pre>
\n = Matches line feed character 
\v = Matches vertical tab character 
\f = Matches form feed character 
\r = Matches carriage return character 
\0 = Matches null character
\ = Matches null character
\0 = Matches null character
</pre>

### octal, hexadecimal, unicode
© in octal is 251
<pre>
\251 => RegExr is <a href="#x">©</a>2014
</pre>

© in hexadecimal is A9
<pre>
\xA9 => RegExr is <a href="#x">©</a>2014
</pre>

© in unicode is 00A9
<pre>
\u00A9 => RegExr is <a href="#x">©</a>2014
</pre>

