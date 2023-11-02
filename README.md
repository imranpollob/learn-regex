# Learn Regex
Examples based regex learning

## Character Handling
### basic match
Match exact characters.

<pre>
men => The <a href="#x">men</a> and wo<a href="#x">men</a>.
</pre>


### [abc] character set
Match any character in the set.

<pre>
[tT]he => <a href="#x">The</a> man and <a href="#x">the</a> woman.
[bc]at => The <a href="#x">cat</a> and the <a href="#x">bat</a> and the rat are having a chat.
</pre>

### [^abc] negated set
Match any character that is not in the set.

<pre>
[^bc]at => The cat and the bat and the <a href="#x">rat</a> are having a c<a href="#x">hat</a>.
</pre>

### [a-z] range set
Match any character between the the two specified character.

<pre>
[0-9] => My ID number is <a href="#x">176584</a>.
</pre>

### . dot operator
Match any character except linebreaks.

<pre>
.at => The <a href="#x">cat</a> and the <a href="#x">bat</a> and the <a href="#x">rat</a> are having a c<a href="#x">hat</a>.
</pre>

Equivalent: [^\n\r]

### \w word
Match any word (alphanumeric and underscore).

<pre>
\w => <a href="#x">PI</a> (π) = <a href="#x">3</a>.<a href="#x">1416</a>
</pre>

Equivalent: [a-zA-Z0-9_]

### \W not word
Match any non word (not alphanumeric and underscore).

<pre>
\W => PI<a href="#x"> π = </a>3<a href="#x">.</a>1416</a>
</pre>

Equivalent: [^a-zA-Z0-9_]

### \d digit
Match any digit.

<pre>
\d => PI (π) = <a href="#x">3</a>.<a href="#x">1416</a>
</pre>

Equivalent: [0-9]

### \D not digit
Match any non digit.

<pre>
\D => <a href="#x">PI (π) = </a>3<a href="#x">.</a>1416
</pre>

Equivalent: [^0-9]

### \s whitespace
Match any whitespace

<pre>
\s => PI<a href="#x"> </a>(π)<a href="#x"> </a>=<a href="#x"> </a>3.1416
</pre>

### \S whitespace
Match any non whitespace

<pre>
\s => <a href="#x">PI</a> <a href="#x">(π)</a> <a href="#x">=</a> <a href="#x">3.1416</a>
</pre>


