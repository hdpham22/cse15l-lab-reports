# Lab Report 5
For this lab report, I used vimdiff to find the different results.<br>
## Different File 1
[This](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/22.md) is the link to the first file<br>
My implementation is correct and the provided implementation is incorrect.
![](images/diff1.png)
My implentation's output is on the left and the provided implementation's output is on the right.
![](images/common1.png)
Expected output: left side of vimdiff screenshot<br>
List of links:<br>
* [foo](/bar\* "ti\*tle")
## Different File 2
[This](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/41.md) is the link to the second file<br>
My implementation is correct and the provided implementation is incorrect.
![](images/diff2.png)
My implentation's output is on the left and the provided implementation's output is on the right.
![](images/common2.png)
Expected output: [url "tit"]<br>
List of links:<br>
* [a](url "tit")