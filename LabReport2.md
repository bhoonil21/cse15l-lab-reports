## part1  ##
![Image](Lab2 PT1.1.png)
![Image](Lab2PT1.2.png)


## Part2 ##
`static double averageWithoutLowest(double[] arr) {
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
  }`
  
 ## Part 3##
 
Week 2 taught me how to use queries in links
Week 3 taught me how to use assertion testing
