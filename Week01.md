#Week 1 Notes#


##Methods##
- Afuction is a collection of code that we can all call by name.
- A method is a fuction that belongs to an object and to acces these methods we use dot notation

##What is an object?##
-An object is a collection of data and methods to operate on those data
  -Specifically an instance of a class.
-An object is responsible for maintaining its state.

##Encapsulation##
- A language mechanism for restricting direct access to some of the object's components.
- A language construct that facilitates the bunding of data with the methods (or fucntions) operating on those data.

##Access Modifiers in Java##
-Public
-Protected 
-Private
-Package-Private

##Codingbat problems##
1. Given 2 strings, return their concatenation, except omit the first char of each. The strings will be at least length 1.


nonStart("Hello", "There") → "ellohere"
nonStart("java", "code") → "avaode"
nonStart("shotl", "java") → "hotlava"

'public String nonStart(String a, String b) {
  return a.substring(1) + b.substring(1);
}'
