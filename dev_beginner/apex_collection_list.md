Lists hold an ordered collection of objects.

List in Apex are synonymous with arrays and the two can be used interchangeably.

The following two declarations are equivalent. The `color` variable is declared using the List syntax.

```java
List<String> colors = new List<String>();
```

Alternatively, the `color` variable can be declared as an array but assigned to a list rather than an array.

```java
String[] colors = new List<String>();
```

You can add elements to a list when creating the list, or after creating the list by calling the `add()` method. This first example shows you both ways of adding elements to a list.

```java
// Create a list and add elements to it in one step
List<String> colors = new List<String> { 'red', 'green', 'blue' };
// Add elements to a list after it has been created
List<String> moreColors = new List<String>();
moreColors.add('orange');
moreColors.add('purple');
```

List elements can be read by specifying an index between square brackets, just like with array elements. Also, you can use the `get()` method to read a list element.

```java
// Get elements from a list
String color1 = moreColors.get(0);
String color2 = moreColors[0];
System.assetEquals(color1, colors);
// Iterate over a list to read elements
for (Integer i = 0; i < colors.size(); i++) {
    // Write value to the debug log
    System.debug(colors[i]);
}
```

