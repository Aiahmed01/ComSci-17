# Title: Matching HTML Tags with Regular Expressions 👋🌎
```md
Introductory paragraph: In this tutorial, we will explore a regular expression that matches HTML tags.
```
## Summary📝
```md
The regex we will be examining is /^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/. This pattern is designed to match HTML tags, both opening and self-closing. We will break down each component of the regex and explain its purpose and functionality.
```
## -Table of Contents-📦 

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)-
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components


### Anchors -⚓
```md
Anchors are special characters that represent the position of the match within the input string. In this regex, we have two anchors:

^ (caret): Matches the start of the string. It ensures that the match starts at the beginning of the string.

$ (dollar sign): Matches the end of the string. It ensures that the match ends at the end of the string.

The combination of ^ and $ anchors ensures that the entire string must match the specified pattern, without any additional characters before or after.
```
### Quantifiers✅
```md

Quantifiers determine how many times a character or group should occur in the match. In this regex, we have the following quantifier:

* (asterisk): Matches zero or more occurrences of the preceding character or group.
The * quantifier is used to match any additional attributes or content inside the HTML tag.
```
### Grouping Constructs 🚧
```md

Grouping constructs allow us to group multiple characters or subexpressions together and treat them as a single unit. In this regex, we have the following group:

([a-z]+): Matches one or more lowercase letters. The parentheses ( ) define the group, and [a-z]+ specifies the character class for matching lowercase letters.
This grouping construct allows us to capture the HTML tag name for further use if needed.
```
### Bracket Expressions 🎗️
```md

In this regex, there are no specific bracket expressions used.
```

### Character Classes 🧑‍🏫 
```md

Character classes allow us to specify a set of characters that should match. In this regex, we have the following character class:

[a-z]: matches any lowercase letter from a to z. This ensures that the HTML tag name consists of one or more lowercase letters.
```

### The OR Operator 📟
```md

The OR operator allows us to specify alternatives for matching. In this regex, we have the following OR operator:

(?:>(.*)<\/\1>|\s+\/>): Matches either the closing tag with inner content or a self-closing tag. The ?: inside the parentheses indicates a non-capturing group, and the pipe | acts as the OR operator.
The first alternative >(.*)<\/\1> matches a closing tag with inner content. The > matches the closing angle bracket, (.*) captures any content inside the tag, <\/\1> matches the closing tag using a backreference to the captured tag name.

The second alternative \s+\/> matches a self-closing tag. \s+ matches one or more whitespace characters, and \/> matches the self-closing angle bracket.
```
### Flags 🚩
```md

In this regex, there are no specific flags used.

```
### Character Escapes 🏃‍♂️ 
```md

In this regex, there are no specific flags used.
```
## Author 🧑 💻
```md

This tutorial was written by Abdulla Ahmed. You can find more projects and code samples on their GitHub profile. For any questions or inquiries, feel free to reach out via email at abdulla@mail.com.
```
