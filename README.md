# Learn Regex
Examples based regex learning

### Character Handling
#### Basic match
Match exact characters.

"men" => "The [cat]() and wo[men]()."

#### [abc] character set
Match any character in the set.

"[bc]at" => "The [cat]() and the [bat]() and the rat are having a chat." <br>
"[tT]he" => [The]() man and [the]() woman. <br>


#### [^abc] negated set
Match any character that is not in the set.

[^bc]at => The cat and the bat and the [rat]() are having a c[hat]().