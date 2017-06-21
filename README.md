Emoji-Ipsum
==========

A Lorem Ipsum generator that's emoji-centric. This is extremely basic, may not work properly on all browsers. More for fun than anything. 

## Documentation

* [`constructor`](#constructor)
* [`genPara()`](#genpara)
* [`genHTML()`](#genhtmltotalparagraphs)
* [`randomInt()`](#randomintmin-max)
* [`capitalizeFirstLetter()`](#capitalizefirstletterstring)
* [`emojiWord()`](#emojiword)
* [`ipsumWord()`](#ipsumword)
* [`genSentence()`](#gensentence)


### `constructor`

Create a new instance of `EmojiIpsum`.

`var emoji = new EmojiIpsum(wordMin, wordMax, wordsPerSentenceMin, wordsPerSentenceMax, paraSentenceMin, paraSentenceMax, emojiRatio);`

All ranges are inclusive.

`wordMin` - Minimum number of letters per word. Defaults to `4`.
`wordMax` - Maximum number of letters per word. Defaults to `8`.
`wordsPerSentenceMin` - Minimum number of words per sentence. Defaults to `8`.
`wordsPerSentenceMax` - Maximum number of words per sentence. Defaults to `16`.
`paraSentenceMin` - Minimum number of sentences per paragraph. Defaults to `3`.
`paraSentenceMax` - Maximum number of sentences per paragraph. Defaults to `6`.
`emojiRatio` - Integer representation of percentage of Ipsum that should be emoji. Defaults to `100`.

### `genPara()`

Returns a paragraph with a random number of sentences between `paraSentenceMin` and `paraSentenceMax`.

### `genHTML(totalParagraphs)`

Returns `totalParagraphs` of Ipsum, with each paragraph wrapped in `<p>` tags.

### `randomInt(min, max)`

Returns a number number in the inclusive range between `min` and `max`.

### `capitaliseFirstLetter(string)`

Capitalizes the first letter of `string` and returns the transformation.

### `emojiWord()`

Generates a word out of emoji HTML entities, and returns it. The word will contain a random number of emoji between `wordMin` and `wordMax`.

### `ipsumWord()`

Returns a random word of latin ipsum. Does not conform to `wordMin` and `wordMax` at the time of writing.

### `genSentence()`

Returns a sentence, with `emojiRatio` percentage of emoji, and a random number of words between `wordsPerSentenceMin`, and `wordsPerSentenceMax`.
