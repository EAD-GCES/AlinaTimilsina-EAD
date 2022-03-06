# Singleton Design Pattern
Singleton Pattern says that just "define a class that has only one instance and provides a global point of access to it". 
In other words, a class must ensure that only single instance should be created and single object can be used by all other classes.

This pattern involves a single class which is responsible to create an object while making sure that only single object gets created. This class provides a way to access its only object which can be accessed directly without need to instantiate the object of the class.

### 2 forms of Singleton Design Pattern:
1. Early initialization:
   - creation of instance at load time
   - easy to use
   - occupies more memory space
2. Lazy initialization:
   - creation of instance when required
  
### Advantage of Singleton Design Pattern
- Saves memory because object is not created at each request. Only single instance is reused again and again.
  
### Usage of Singleton Design Pattern
- Singleton pattern is mostly used in multi-threaded and database applications. It is used in logging, caching, thread pools, configuration settings etc.
