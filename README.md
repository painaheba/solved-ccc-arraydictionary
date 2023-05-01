Download Link: https://assignmentchef.com/product/solved-ccc-arraydictionary
<br>
Remove from ArrayDictionary

The ArrayDictionary class implements the Dictionary interface as a dictionary with chaining capability for key collision.

The hash function of this class is:

private int hashFunction(String key) {

// not ideal

return key. length();

As stated in the comment, this is not the most capable solution for a hash function but it helps us test the knowledge Of the hash key vs

entry key. “Hash key” is the integer value (return value Of the hash function) produced by passing the entry key through the hash function. If

multiple entry keys have the same hash key, these entries will be •chained” under the same hash key. Here’s an example:

dictionary [e]

dictionary[ll

dictionary 12]

dictionary [3]

dictionary(41

dictionary [5]

null

= 18283)}

= {Cal, 00112233)}

= {(ron, 456))

{(tony, 123)}

{(katie, 1122)}

“tony” and “alex” both have the same hash key 4 because both are 4 character long, and therefore they are chained (much like in a single

linked list) in dictionary[4J.

Write the code to implement the remove function.

@Override

public void remove(String key) {

// homework

This function removes a key value pair in the dictionary by it’s key if it exists. No-op if otherwise. Tests are provided. Notice the key in the

parameter is the entry key, not the hash key. All tests are provided and should pass upon correct completion.