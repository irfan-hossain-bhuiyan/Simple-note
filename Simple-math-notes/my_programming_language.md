In ecs,a basic implementation is something like,
```python
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
another approch is meta programming.

## Dynamic set type:
Each time I add a element in an array,other than doing some hashmap shinagenan,
We will add the boolean in the struct,that act as if the element exist in the set or not.If there 
are multiple set to use,We could use a bitmap for it.
    
