What’s the difference between a static and an instance constructor?
Static constructors allow you to initialize static variables in a class or perform other operations required in a class after it is first referenced in code. They are called only once per program run.

Whenever you create a new object (an instance of a class), the instance constructor is called.


How does the use of a static constructor differ from setting properties/values?
Static class members, which are shared by all instances of the class, are initialized via a static constructor. It operates at the class level and is automatically run prior to any access to static members. On the other hand, you may modify the characteristics or values of specific instances of a class by setting properties or values. Instead of the state of the entire class, it impacts the state of those particular objects. The primary distinction is that altering properties or values affects the state of individual objects, whereas a static constructor initializes shared elements.

Knowing what you now know about the stack and the heap, how might you rethink the way you did projects in previous courses, to make more effecient use of memory?

By understanding the stack and heap, we can optimize how projects use memory. Allocating small, transitory items on the stack, which is quicker for memory allocation and deallocation, is one technique to do this. Using the heap is preferable for items with longer lifespans or that are bigger. To prevent memory leaks and excessive memory utilization, heap memory management is crucial. We can use memory in our projects more effectively by taking into account the size and lifespan of things.

4. Compare “Garbage Collection” in C# with the lifecycle of normal household items.


If we don't require anything, we discard it with C#'s garbage collection system. Similar to emptying a trash can, the garbage collector locates and eliminates unneeded things from memory. By automating memory deallocation, it reduces manual administration and guards against memory leaks. The trash collector in C# maintains memory organized without manual disposal, much as garbage collection keeps our houses tidy.
