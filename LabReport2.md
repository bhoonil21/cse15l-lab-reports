## part1  ##
![Image](Lab2PT1.1.png)
This code calls the url.getPath() method which gets the path of the url and then it uses .contains to check whether the path has /add-message
The code url.getQuery().split() gets the query from after the / and then delimts it into components of an array via spliting it with the "=" sign 
The array is then checked for the "s" argument via using the arrays first index .equals("s") and then if the array that was formed by split contains it, the element after is added to the list which is is then returned to the page. 
The values of the query are dependent on what the user types in to the query field of the url, which then affects the parameters[] array by changing the parameters[1] to whatever the second String passed in is after the = sign. In this case it goes from "Hello" to "How are you"

![Image](Lab2PT1.2.png)


## Part2 ##

Failure inducing output
```
@Test
  public void testAverage() {
    double[] input1 = {2,2,5, 6,7 };
    assertEquals(6, ArrayExamples.averageWithoutLowest(input1),0.00000001);
  }
```

Non-Failure inducing output
```
@Test
  public void testAverage() {
    double[] input1 = {2,5, 6,7 };
    assertEquals(5, ArrayExamples.averageWithoutLowest(input1),0.00000001);
  }
```




BEFORE BUG FIX
```
  static double averageWithoutLowest(double[] arr) {
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
    }
    return sum / (arr.length - 1);
  }
```

AFTER BUG FIX
```
static double averageWithoutLowest(double[] arr) {
    int countLowestoccurences =0;
    if(arr.length < 2) { return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { sum += num; }
      else{
        countLowestoccurences+=1;
      }
    }
    return sum / (arr.length - countLowestoccurences);
  }
  ```
  
  
  
  
 ## Part 3##
 
Week 2 taught me how to use queries in links
Week 3 taught me how to use assertion testing
