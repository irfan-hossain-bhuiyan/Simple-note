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
another approch is my compile 
    
