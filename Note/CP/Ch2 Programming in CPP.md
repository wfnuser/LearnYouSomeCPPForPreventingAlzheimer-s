# Programming in C++

- fast
- standard code libraries
- error management is terrble

## Environment
in macOS you can use XCode

## Hello world

```
1 #include <iostream>
2
3 using namespace std;
4
5 int main() {
6 // Print Hello World!
7 cout << "Hello World!" << endl;
8 }
```

iostream - input and output stream
using namespace std - 不用每次都写namespace

## 变量和类型
int five = 5 声明变量+类型

string int float double char bool

可以用 auto 推导类型


### functions
函数包括参数、类型、返回值和函数体。
C++里函数调用的时候传参数传的是值，意味着所有的参数都会拷贝一份。在函数中修改参数本身并不会影响原始的变量。
函数可以是void的，但依旧可以对外部产生影响。（这并不是一个好想法）
有两种方式：1. 修改全局变量 2. 传递引用或者指针

### struct
结构体是一种特殊的类型，可以将信息按照用户指定的方式组合起来。
结构体可以有构造函数。
结构体下面也可以定义方法。

```
What happens if we try to change a member variable in a const member function?
"cannot assign to non-static data member within const member function"
```