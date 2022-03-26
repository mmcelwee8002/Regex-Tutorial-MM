# Regex-Tutorial-MM

Introductory paragraph (replace this with your text)

## For this challenge I will be creating a totorial about Regex.  Specifically I will be evaluating the regex:  
## /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This is used for matching an email



## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Boundaries](#boundaries)
- [Bracket Expressions](#bracket-expressions)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This is used to find and identify an email.
### Anchors
Anchors are used in a few place.  Most notibly they are used at the beginning of the expression as well as at the end. in this case it is matching ^ as well as $

### Quantifiers

A qualifier is used to identify a character or group of characters to use or exclude.  In the email exapmle the "+" is used to let tell the expression that any and all character configuration prior to the "+" can be used. A qualifier can also be used with {} curly braces.  This is telling an exact match of characters.  In this case inside the curly braces it is saying after the "." character the last set must have between 2-6 characters {2,6}.

a ? is another qualifier that we aren't using in this exapmple but that would be used as "optional"  so if we had the word that was spelled two ways for example:  glamour / glamor the "u" character could or couldn't be there and both was are acceptable.  So that would be written glamou?r telling us "u" is optional.


### OR Operator
Operators in a regex is used to build out groups or sets of groups.  In our example the () is used 3 times to tell us there are three groups to be examined.  Within each group we use [] to itentify the specific characters used within these groups.  {} is also an oporator as well as ^ and $ which were examined earlier.

### Character Classes
Character classes are exactly what they seem.  Different characters that can be used and in different ways.  Alpha numeric (a-z) or special characters.  We can also use operators to use or exclude certain characters.  For example [a-f] would look for all characters within the range of a-f however [^a-f] would exclude all characters a-f.  we can use various anchors and qualifiers to look for or ignore certain characters.  In our case with email the "\." as mentioned is looking for and excepting the "." character.

In our email example the "@" and "." symbols are used outside of operators and qualifiers.  This is saying between group 1 and group 2 there needs to be a "@" and between group 2 and 3 there needs to be a "." as would be custom to an email address.
### Flags
Flags are used to change how the expression is seen.  To look at case of a character or to ignore the case.  mulitline or single line.  All words or some words.  Using or not using flags will render different results
### Grouping and Capturing
As mentioned before groups are used with the () and capture with the [].  This is saying there are 3 groups represented by () and with in those groups 3 sets that are being captured.

### Boundaries
Another way an anchor could be used as \.  This could be used to indcate a word boundary (the end of the word) so s\b would find all the "s" character a the end of the word while s\B would find all the "s" characters regardless of location.

In the email example above \. is used to indicate that if there is a "." character it can use it


## Author

My name is Matthew and I am working toward a developer.  I am curntly a product owner with asperations in development.  
