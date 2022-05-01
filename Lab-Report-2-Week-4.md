# Week 4 Lab Report
[Index](https://lillyjrjy.github.io/-cse15l-lab-reports/index.html)
## Error1
---

<img width="1231" alt="Screen Shot 2022-04-22 at 7 39 07 PM" src="https://user-images.githubusercontent.com/56412294/164868949-bc58e327-2b81-4b5c-b16f-0bac81788a40.png">

[File that induced an error](https://lillyjrjy.github.io/-cse15l-lab-reports/nothing.html)

error message
<img width="597" alt="Screen Shot 2022-04-24 at 1 28 29 AM" src="https://user-images.githubusercontent.com/56412294/164967492-eeb76be7-4772-46d3-b0ca-98d82f8ec600.png">

The input file contains only the link with no brakets. When getLink can't find any bracket, indexOf will return -1, which will brake our code when it tries to use -1 as an index for the substring, which lead to seeing the StringIndexOutOfBoundsException, the symptom.

## Error2
---

<img width="728" alt="Screen Shot 2022-04-24 at 1 47 39 AM" src="https://user-images.githubusercontent.com/56412294/164968294-dc053318-2f33-401e-9265-c9fcdad13edf.png">


[File that induced the error](https://lillyjrjy.github.io/-cse15l-lab-reports/aNewFile.html)

error message
<img width="525" alt="Screen Shot 2022-04-24 at 1 48 10 AM" src="https://user-images.githubusercontent.com/56412294/164968320-38458652-f045-4609-b50e-b8b3d59ac348.png">

There is a space at the end of the file, because the index of last parenthesis+1 isn't the length, the method reached a infinite loop. The loop stops when java run out of space. Therefore, an error of OutOfMemory.



## Error3
---
<img width="799" alt="Screen Shot 2022-04-24 at 1 59 53 AM" src="https://user-images.githubusercontent.com/56412294/164968728-5c28dca4-eb6b-455b-83e3-55c16c5de913.png">


[File that induced an error](https://lillyjrjy.github.io/-cse15l-lab-reports/cat.html)


output 


The method can't distinguish between an image and a link. When we used an image in the file, the method returned the link for the image, which is not what we wanted.