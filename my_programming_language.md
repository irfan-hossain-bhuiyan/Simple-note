In ecs,a basic implementation is something like
```rust
trait object{
    func draw();
    func ready();
    func update();
}
let objects:Vec<dyn<object>>;
for x in objects:
    x.ready()
for x in objects:
    x.update();
    x.draw();
```
but it has a big drawback,it has to jump through the pointer,so not a pure ecs.
What I need is a dynamic sized type,a typed union which is automatically set to max size ,
another approch is my compile evaluation,like 
```
let allVec<>={
    const types:Vec<type_id>;
    const Vectypes:Vec<Vec<type_id>>;
    fn new(){return this;}
    fn pushback(comptime T value){
        comptime{if(types.contains())}
        
    }
}
```
## The problem I am having:
While making logic gate simulator in raylib,I made a basic ecs system having every object that want to run per frame have an update method,now I want to made a dragable and movable class that after inheriting by other class can be dragged by mouse and moved by keyboard and also run the update method per frame.

### Things I want in my programming language
1. let's say I have a 
```cpp
class A{
    String s;
    int a;
    int b;
    int c;
}
```
Now I want when I want a function that will ensure the mutate of all the integer value,I can do something like,
```cpp
class A{
    void mutate_all(int A,int B,int C){
        a=A;b=B;c=C;
    }
}
```
but then absent mindly I added another int
```cpp
class A{
    int a;
    int b;
    int c;
    int d;
}
```
it is very possible,I will forget it in mutate_all function,how can I fix it?
I want something like a compile time check to ensure,so the code doesn't look garbage.

2. Let's say a object updates in a game,I want other object to mutate when the object updates.
In a standard way is to do,
```cpp
class objectA{
    void mutate();
}

class objectB{
    objectA *other;
    void update(){
        other->mutate();
    }
}
```
Now the problem with this approch is that we have  no idea to 
know when the objectA will mutate just looking at the objectA class,We have to read 
all files to see where the objectA is referenced.
One way to fix this problem is like
```cpp
class objectA{
    objectB b;
    objectA(){b->funcVec.push_back(this->mutate);}
    void mutate();
}
class objectB{
    vector<function<void()>> funcVec;
    void update(){
        for(auto x:funcVec){x();}
    }
}

```
