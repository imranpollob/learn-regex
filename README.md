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