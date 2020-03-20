# Java

## Coding Tips

### General 

- Java doesn't manage multi-inheritance
- Every class has implicitly an empty constructor
- `java.lang` is implicitly in every class
- The garbage collector doesn't dispose primitive variables, only objects. Objects inside
a class are also disposed.
- `StringBuilder` manages strings in a single memory location when it is edited.
- `String` manages strings in multiple memory locations every time it is edited.
- Method's params are sent by reference if they are objects, primitives are sent by value
- `private` methods and attributes can be accessed from a class that contains it
- The default constructor is removed if there is another empty constructor
- Methods in implicit interfaces are public


### Data Types

- Every data type that isn't a primitive is an Object
- Arrays can be written like this: `...` and `[ ]`
- Primitive types cannot be assigned null, their Object form does
- Primitive types can be initialized in methods, not when they are outside


- Octal values are stored in integers. eg. 014 = 12
- Hexadecimal values are stored in integers. eg. 0xC = 12
- Strings containing numbers must be converted according to the letter appended at the end.
eg. Double.valueOf("120D") Double.parseDouble("20D")


- The result of ecuations are stored in a memory location with the largest operator size
- Bytes, chars and shorts are automatically promoted to integer before operating them
- Literal decimals are interpreted as if they were doubles, even if they are assigned to a float


### Operations

- `i++` does the operation after getting the value
- `++i` does the operation before getting the value
- In a `for` the declaration part can be omitted. eg. `for(; x < 1; x++)`

### Keywords

- A `final` variable can only be initialized in the constructor
- Using `final` on methods, disallow overrides in inherited classes
- Using `final` on classes, disallow classes to inherit from it


- The garbage collector doesn't free up space of `static` variables
- `static` variables reserve memory space since the program starts
- `static` imports only import static variables and methods
- `static` blocks are used for assigning values to `static` variables. It works similarly
as a constructor. It only executes once, when the value is called. `static {    }`
- `static` methods cannot be overrode


- `break` stops the iterations on a loop
- `continue` skips the current iteration on a loop, and continues with the next iterations
- `continue` can use labels to continue from them `label:`, but it is considered as a bad practice


- `case` in switches doesn't compare variables, only compares `final` variables

### Exceptions

- Both RuntimeException and Error are unchecked exceptions

### Advanced

- Reflection gets methods and attributes of unknown classes. (JPA implements it)
- The `finalize()` method is implicitly inside the Object class. It is called before the 
garbage collector disposes it
- If the `hashCode()` method is overrode, then the `equals()` method should be changed too
- Constructors can call other constructors from their same class, using "Chaining":
`this(@type @name...)`

