# mnsecretjsninja2ed
## Chapter 7. Object orientation with prototypes
- Every function has a prototype object that’s automatically set as 
the prototype of the objects created with that function.
- When the function is created, it immediately gets a new object assigned to its prototype object
- When we use a function as a constructor (for example, by calling new Ninja()), the prototype of the newly constructed object is set to the object referenced by the constructor function’s prototype.
### 7.2.1. Instance properties
Figure 7.7. After construction, ninja1 has the property swung, and its prototype is the Ninja prototype that has only a constructor property.

(TBU)
Done.
need to do exercise.



## Chapter 12. Working the DOM
interpret self closing tags.
```
const tags= /^(area|base|br|col|embed|hr|img|input|keygen|link|menuitem|meta|param|source|track|wbr)$/i;
function convert(html){
  return html.replace(/(<(\w+)[^>]*?)\/>/g,(all,front,tag)=>{
    return tags.test(tag)?all:front+"></"+tag+">";
  })
}
```

### 12.2. Using DOM attributes and properties
```
e.getAttribute('id')
e.id
```
that the property and attribute are sharing the same value—they aren’t.
