# Week 2 Notes #

## Compering content ##
- Do not use == to compare content
- How do we compare content?
  1. Null and/or actual string
  2. length
  3. ASCII values

## @Override ##
- @Override is an annotation, like @Test
- It tells the interpreter that we are implementing our own version of an inherited method.

## Inheritance ##
- In java Inheritance refers to two things
    - Either extending a class or implementing an interface
- Inheritance is a method by which one class can access all the public or protected methods and fields of a parent object
- Additionally, all objects can be grouped by their parent
- Inheritance lets us re-use code in a meaningful way

## Codingbat Problems ##
1. Given a string, return a string where for every char in the original, there are two chars.


- doubleChar("The") → "TThhee"
- doubleChar("AAbb") → "AAAAbbbb"
- doubleChar("Hi-There") → "HHii--TThheerree"

```java
public String doubleChar(String str) {
  String result = "";
  
  for(int i = 0; i < str.length(); i++) {
    String letter = str.substring(i, i + 1);
    
    result = result + letter+ letter;
  }
  
  return result;
}
```

2. Return the number of times that the string "hi" appears anywhere in the given string.


- countHi("abc hi ho") → 1
- countHi("ABChi hi") → 2
- countHi("hihi") → 2

```java
public int countHi(String str) {
  int count = 0;
  
  for(int i = 0; i < str.length() - 1; i++) {
    String pair = str.substring(i, i + 2);
    
    if (pair.equals("hi")) {
      count++;
    }
  }
  return count;
}

  
