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

## Explore More

Suppose that once you received a request from one of your friends, he told you he was a photography beginner and needed some great photos to learn. 

But he found visiting the website every time is too complicated and asked you if you can download all the images from the websites automatically.

In python, this is easy by its rich third party libraries. 

1. First, download what we need from the command line:
```python
pip install requests   #For request the website
pip install bs4   #For get the img
```
For we are not teaching python, code below:
```python
import requests
from bs4 import BeautifulSoup


response = requests.get(url, timeout=20)   #get it
soup = BeautifulSoup(response.text, "lxml")   #analysis it
img_list = soup.find_all("img")   #find images

for img in img_list:   #get one
	img_url = img["src"]   #images src
    try:   
		img_get = requests.get(img_url, timeout=20)   #get image
	else:
		name = int(time.time())   #time now
		with open(path + "\\" + str(name) + choice.get(), "wb") as f:   #open file
			f.write(img_get.content)   #write image
    except Exception:
        continue   #next image
```
If you calm down and read it. You will find the code is really readable for humans! It’s really easy! Only 15 lines!
```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```

```python

```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE4NjMxMDQ2MDBdfQ==
-->