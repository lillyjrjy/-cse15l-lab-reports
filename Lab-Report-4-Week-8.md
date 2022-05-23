# Week 8 Lab Report
[Index](https://lillyjrjy.github.io/-cse15l-lab-reports/index.html)

## epositories
Repository we worked: https://github.com/YoavGutmanUCSD/markdown-parser-2

Repository we reviewed: https://github.com/DanUCSD/markdown-parser.git

---------
## Expected output:
1. 
```[`google.com, google.com, ucsd.edu]```

2. 
```[a.com, a.com(()), example.com]```

3. 
```[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule, https://cse.ucsd.edu/]```

-----
## Tests:
<img width="559" alt="image" src="https://user-images.githubusercontent.com/56412294/169743394-c9d439cf-ad08-48e6-b470-59a0601e74ac.png">

## Our Implementation results

1. 
 <img width="980" alt="Screen Shot 2022-05-22 at 9 34 10 PM" src="https://user-images.githubusercontent.com/56412294/169743935-cbc974ce-6a46-488b-8dce-7d7253b3845f.png">

 Our code also read the first line in the snippet. An easy way is to treat the "`" like "!", and remove the link when it was found in front of "["

2. 
<img width="983" alt="Screen Shot 2022-05-22 at 9 34 55 PM" src="https://user-images.githubusercontent.com/56412294/169744016-a07b0e32-12c5-4d29-8cbb-485d46bb1b5f.png">
Our code stopped reading any link after the first ")" was found. This issue is more complacated as to the code has to decide with parenthsis should be taken in as the output itself. We might need to incorporate a stack adt.

3. 
<img width="977" alt="Screen Shot 2022-05-22 at 9 35 33 PM" src="https://user-images.githubusercontent.com/56412294/169744080-d6a71b2b-a3c0-496e-bc75-95f735df2259.png">

I do, the problem with our output is that we included empty spaces, which could easily be fixed with ```replaceAll("\\s","")```


## Implementation of the other group results

1. 
2. 
3. 