# Regex Tutorial Starter Code- MATCHING AN EMAIL 

# Description

Greetings and welcome to this extensive guide on how to match an email address/ email addresses by using REGULAR EXPRESSIONS or REGEX. We will be using REGEX with a popular coding language known as JavaScript. By the end of this tutorial, all beginner and advanced software developers will be very knowledgeable of this subject. They will all have a full understanding of the significant components. This will be achieved through detailed explanations and analysis of examples. The focus of this tutorial is email regex. This is where we will examine the different parts of a regex pattern that's intended for validating email addresses, highlighitng the importance of each element ensuring the process is precise and trustworthy.

# Table of Contents

* What is Regex?
* Quantifiers
* Grouping Constructs
* Character Classes
* Links 
* Credit

# What is Regex?

 REGEX is a sequence of characters that defines a search pattern for a text. This also comes from the mathematical concepts of regular sets.  This is a code that can search for things like phone numbers, URLS, email addresses (in our case), etc.  With this, you can search for words that start with a certain letter, numbers that follow a certain format, or symbols that display in a particular order. Once the developer has their code, they can use it to successfully search through any text file or document. 

 # Quantifiers

 Quantifiers? Not Quantum Physics, quantifiers! When a developer uses regex quantifers are important for determine a maximum number of times a pattern should match. These are added after a character, char class, or group. The plus sign for instance means "one or more". It is used after a pattern to inidicate that it should occur atleast once but can appear consecutively several times. The {2,6} quantifier, on the other hand, specifies that a pattern should occur atleast once but can appear consecutively several times. The {2,6} quantifier specifies that a pattern should occur between 2-6 times. 

 For example the regex: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ matches a valid email address that starts with one or more lowercase letters, digits, lowercase letters, hypens, dots, all followed by a period and a 2-6 top level domain. 

 * Quantifier 
 (+) : This matches one or more
 (*) : This means 0 or more
 (?) : This means 0 or 1 

([a-z0-9_\.-]+): This matches one one or more lower case letters, digits, underscores, dots, or hyphens.
([\da-z\.-]+) : This matches one or more digits, lowercase letters or dots.

# Grouping Constructs

When writing a regular expression, you may need to group certain characters or sub expressions together. This is where grouping constructs come in handy. They allow you to treat multiple characters as a single unit within the expression, which can be helpful for applying quantifiers or alternation, capturing parts of the match for later use. By creating a group , simply enclose the desired characters or sub expression within the parentheses (). In our regex pattern /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, we have three groups enclosed in (), which captures a different part of the email address.

In email addresses, there are three different parts that can be captured by grouping constructs: the Local-Part, the Domain, and the Top-Level Domain.

* Local Part:

 it is the username part of the email address that appears before the @ ymbol. This group ensures that the username follows a valid format by matching characters that can be lower/uppercase letters, numbers, underscores, dots, and hypens. This represents the part of the email address that comes after the @ symbol and before the final (.). This helps create a valid format.

* Domain Group:

matches the domain name of the email address and can include lower/upper case letters, numbers, dots, and hypens. For instance the email address: "Mizael.Gonz47@sub-domain123.example.com" has a Domain of  "sub-domain123.example.com that matches the regez pattern ([\da-z.-]+) bc it contains  lower/upper case letters, numbers, dots, and hypens.


* Top-Level Domain:
this group aligns with and matches the Top Level Domain of the email address which can be only valid top level domains between 2-6 characters. For example "Mizael.Gonz47@sub-domain123.example.com has a TOp Level Domain of com, which matches the regex pattern ([a-z.]{2,6}) because it only contains lowercase letters and a length of 3 characters. 


# Character Classes

The pattern uses char sets like [a-z] [0-9], and [-] to represent multiple characters, allowing a single character match from the specified range. For example, /[a-zA-Z0-9]/ matches a single alpha numeric character that can be an uppercase/lowercase letter or digit. Inside the char sets, metacharacters like 9.0 dot lose their special meaning are treated as literals. In the email regex pattern, the hypen (-) is used as a literal character without escaping when placed at the beginning or end of the char set. A char set like [\da-z\.-] matches a single digit, an uppercase/lowercase letter, period, comma, and hypen. The character classes \d,[A-Z], and [a-z] match the digits, uppercase/lowercase letters respectfully. The metacharacters . & - are treated as literals since they're placed inside the char class without any special meaning. 

# Links


# Credits

Youtube: https://www.youtube.com/watch?v=aCdKx__VabQ,
Youtube: https://www.youtube.com/watch?v=QxjAOSUQjP0