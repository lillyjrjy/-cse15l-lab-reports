# Week 8 Lab Report
[Index](https://lillyjrjy.github.io/-cse15l-lab-reports/index.html)


Found the difference using ```vimdiff``` by comparing the two results.txt files.

## test1
<img width="943" alt="image" src="https://user-images.githubusercontent.com/56412294/172040650-59faf357-897e-4123-8afe-e414eccfdab0.png">

[Test link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/12.md)

expected output:

<img width="648" alt="Screen Shot 2022-06-05 at 1 27 07 AM" src="https://user-images.githubusercontent.com/56412294/172042153-30c92979-403b-4bb1-ba5a-4af5da851089.png">



The provided program is right


our program didn't find an open parenthesis, so openparen returns -1, the substring it read is from index -1+1 to the close parenthesis, which is why it give the string output.

------
## test2
<img width="909" alt="image" src="https://user-images.githubusercontent.com/56412294/172040665-ad9b91a0-c09f-4261-b59b-83b1dd8cba7e.png">


[Test link](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/494.md)

expected output:

<img width="648" alt="image" src="https://user-images.githubusercontent.com/56412294/172043558-a10ce276-518b-4665-aef2-6a66e889853f.png">



both are wrong

our program reads everything in the outter set of parenthesis, it didn't ignore the "\" because we didn't have any code for case like this one. 
