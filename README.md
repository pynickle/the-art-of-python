# the-art-of-python
Feel the charm of Python! Let us love python together!

Python, being a well-designed high-level programming language, provides us with many features for the programmer's comfort. It also be known for “built-in batteries” because of its various and rich standard libraries and built-in functions. 

Why not study it? l will try to make you feel the charm of python from the bottom of your heart.

## Get Started

First, let us start with the classic example - HelloWorld. In python, Hello World is like this:

```python
print("Hello,World!")
```
One line. And in Java:
```Java
public class HelloWorld {
    public static void main(String []args) {
       System.out.println("Hello,World!");
    }
}
```
5 lines. In C programming language:
```C
#include <stdio.h>
int main(){
   printf("Hello,World!\n");  
   return 0;
}
```
5 lines, the same as Java. If this is not enough for you to believe python, another example below:

The question asks you to use a string character for string concat.

Such as, an array like this: “Hello”, “World”. The join method should return “Hello World”. In Java, we don’t have a method Java has written for us:
```Java
import java.util.ArrayList;
import java.util.List;
public class Join {
    public static String join(String join,String[] strAry){
        StringBuffer sb=new StringBuffer();
        for(int i=0;i<strAry.length;i++){
             if(i==(strAry.length-1)){
                 sb.append(strAry[i]);
             }else{
                 sb.append(strAry[i]).append(join);
             }
        }
		return new String(sb);
	}
	public static void main(String[] args){
        String[] sa={"Hello", "World"};
        String a=join(" ",sa);
        System.out.println(a);
    }
}
```
But in python. Python team has writen the method join for us:
```python
a = ["Hello", "World"]
print(" ".join(a))
```
The line numbers is very different. As we all see, python is more simple than java. That’s why it has “built-in batteries”.

## Python Package
Python also welcomes us to provide more useful packages on pypi. There are many great packages for us to use.

Here are some of them:

- requests : get any website
- django : make your own website
- keras : for deep learning
- numpy : scientific calculation

And more is waiting for your explore.
Go to [pypi.org](https://pypi.org) to find more!

## Explore More

Suppose that once you received a request from one of your friends, he told you he was a photography beginner and needed some great photos to learn. 

But he found visiting the website every time is too complicated and asked you if you can download all the images from the websites automatically.

In python, this is easy by its rich third party libraries. 

1. First, download what we need from the command line:
```bash
pip install requests   #For request the website
pip install bs4   #For get the img
```
For we are not teaching python, code below:
```python
import requests
from bs4 import BeautifulSoup
import time   #a standard library for timing


response = requests.get(url, timeout=20)   #get it
soup = BeautifulSoup(response.text, "lxml")   #analysis it
img_list = soup.find_all("img")   #find images

for img in img_list:   #get one
	img_url = img["src"]   #get images src
    try:   
		img_get = requests.get(img_url, timeout=20)   #get image
	else:
		name = int(time.time())   #record time now for file name
		with open(path + "\\" + str(name) + choice.get(), "wb") as f:   #open file in binary form
			f.write(img_get.content)   #write image info to file
    except Exception:
        continue   #error occured and jump to next image
```
Even though you haven’t studied python, if you be calm and read it. You will find the code is really human-readable! It’s really easy! Only 15 lines!

## Expert Python3

Python is created by Guido Van Rossum in 1991. It has a long history. During the long time, it never gives up developing python greater, and it makes today’s popular python. It has many things other languages do not support.

Now we are going to expert python more deeply. See how great it is!

First, let us start with decorator. Suppose that you are discovering which is more efficient, join() or +. If you do not use decorator:
```python
import time   #time module
def time_c(func):
	start = time.time()   #time now
	func   #run function
	print(f"Time used: {time.time()-start}")   #print result
def sleep1(a, b):
	print(a, b)   #function that has parameters
	time.sleep(2)   #little sleep 
time_c(sleep1(1,2))
```
It has a poor readability. So decorator appeared in the world of python:
```python
def time_c(func):   #decorator begin
    def wrapper(*args, **kwargs):   #inner code there
        start = time.time()   #record time now
        func(*args, **kwargs)   #run function with parameters
        elapsed = (time.time() - start)   #record end time
        print("{} : Time used: {}".format(func.__name__, elapsed))   #print result
    return wrapper   #return inner function
@time_c   #use the decorator with @
def sleep2(a, b):
	print(a, b)
	time.sleep(2)
sleep2(1,2)
```
We use @ to use a decorator. It improves the code quality. That’s what python brings us. Just a little part.

Python also supplies us with a beautiful way to print. We do not need to use incomprehensible %.

Format method is provided. Like below code:
```python
name = "nick"
print("my name is {}".format(name))   #use {}
print("my name is {0}".format(name))   #use {0}
print("my name is {name}".format(name=name))   #use{name}
```
A more gentle way is to use f for simple format:
```python
name = "nick"
print(f"my name is {name}")
```
That is really human-readable.Python has improved much during these years.

## Use Python

Python, with its various third party libraries on pypi. It can help us do many things. 

For example, there are many web framework on pypi. With these powerful technology, we can make great website. There is some:

- django : much bigger
- flask : more flexible
- tornado : an asynchronous library
- falcon : a fast network library
- pyramid : proper weight

So many! l don't know which to choose! Then l will list some uses of python. Enjoy!

- scientific calculation
- web development
- web spider
- data analysis
- artificial intelligence
- GUI game
- GUI programming
- data visualization

If you want to see more information about python packages. See awesome-python on GitHub:

- [awesome-python](https://github.com/vinta/awesome-python) : English
- [awesome-python-cn](https://github.com/jobbole/awesome-python-cn) : Chinese

And l hope my own project can help with the further python study(study_program, interesting_program and what_the_f*ck folder):

[amazing-python](https://github.com/pynickle/amazing-python)

wtfpython is a good project, too. Hope you can learn something interesting from it:

- [wtfpython](https://github.com/satwikkansal/wtfpython)
- [wtfpython-cn](https://github.com/leisurelicht/wtfpython-cn)
