##Javascript engine
- Javascript engine has many releases
- [V8, SpiderMokey] they are one of many

![Image text](images/js%20engine.png)
пример работы AST [https://astexplorer.net/](https://astexplorer.net/)
##Javascript runtime
##Interpreter/Compiler/JIT Compiler
interpreter vs compiler

Just In Time Compiler 

#####Javascript is an interpreted language
I mean, yes, initially when JavaScript first came out, you had JavaScript engines such as Spider Monkey created by Brendan Eich that interpreted JavaScript to bytecode.

And that engine was able to run inside of our browsers to tell our computers what to do. 

But things have evolved. Now we don't have just interpreters. We also use compilers to optimize this code.

So this is a common misconception when somebody says JavaScript is an interpreted language. 

Yes, there is some truth to it. But it actually depends on the implementation, you can make an implementation of JavaScript, of the JavaScript engine that perhaps only compiles.

##Writing optimized code
Нарушают оптимизацию 
- eval()
- arguments
- for in
- with
- delete

#####Inline cashing
```
function findUser(user) {
    return 'found ${user.fistName} ${user.lastName}';
}

const userData = {
    firstName: 'Johnson',
    lasrName: 'Junior'
}

findUser(userData); //если JIT Compiler имеет доступ к userData на етапе оптимизации то 
                    //компилятор заменит вызов функции на результат его выпонения 
//'found Johnson Junior'
```
#####Hidden classes
```
function Animal(x, y) {
    this.x = x;
    this.y = y;
}
const obj1 = new Animal(1, 2);
const obj2 = new Animal(3, 4);
obj.a = 30;
obj.b = 100;
obj.b = 30;
obj.a = 100;

```

##Call stack + Memory Heap
##Stack Overflow + Memory Leaks
##Garbage Collection
##Node.js
##Single Threaded Model



