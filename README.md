# Learn Regex
Examples based regex learning

## Character Handling
### Basic match
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
</pre>\