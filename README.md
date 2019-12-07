# Learning advanced features introduced since C++11

Here is the list of items that have been introduced in C++11 and are frequently asked in Interviews of many Investment Banks.

First follow this [link](http://www.codeproject.com/Articles/570638/Ten-Cplusplus-Features-Every-Cplusplus-Developer) to see some of the most important features that have been introduced as a part of C++11 and are frequently being used and being more precise must be used in all modern C++ applications.

Now are following are the topics that you should prepare without fail.

1. **Move Semantics** - This is an important feature and you must understand how it works and why it is useful. Refer the links below.
   - <http://www.cprogramming.com/c++11/rvalue-references-and-move-semantics-in-c++11.html>
   - <http://stackoverflow.com/questions/3106110/what-are-move-semantics>
   - <http://www.codeproject.com/Articles/397492/Move-Semantics-and-Perfect-Forwarding-in-Cplusplus>
   - <http://www.cplusplus.com/reference/utility/move/?kw=move>
2. **New Data Structures**
   1. **Forward List**
      - <http://www.cplusplus.com/reference/forward_list/forward_list/>
   2. **Unordered Map `(Extremly Important)`,Set, Multimap**
      - <http://www.cplusplus.com/reference/unordered_map/unordered_map/>
      - <http://stackoverflow.com/questions/21518704/how-does-c-stl-unordered-map-resolve-collisions>
      - <http://stackoverflow.com/questions/11337494/c-stl-unordered-map-implementation-reference-validity>
   3. **Array**
      - <http://www.cplusplus.com/reference/array/array/>
3. **Multi Threading `(Very Important)`** - Always remember the C++11 Multi threading is just a OOPs based wrapper on pthread and is totally dependent on pthread library and hence you must have to link the pthread library with the code by add "-lpthread" to your makefile for compilation. Please google to see how to use them as there are plenty of examples available. I will send a my implementation of Ring Buffer code later which uses a lot of the C++11 features.
   1. **Atomic `(Extremely Important)`** - <http://www.cplusplus.com/reference/atomic/>
   2. **Thread** - <http://www.cplusplus.com/reference/thread/thread/>
   3. **Mutex** - <http://www.cplusplus.com/reference/mutex/>
   4. **Conditional Variable** - <http://www.cplusplus.com/reference/condition_variable/condition_variable/>
   5. **Thread Local Storage `(Very Important)`** - <http://en.cppreference.com/w/cpp/language/storage_duration>
4. **Smart Pointers `(Extremely Important)`** - You must understand clearly how these Smart Pointers are implemented internally. Refer this [link](http://www.codeproject.com/Articles/15351/Implementing-a-simple-smart-pointer-in-c). This implementation has few bugs but you will be able to understand the basic idea of how are they implemented and how they work.
   1. **Auto Pointer** - Remember this is deprecated in C++11 and have been replaced with Unique Pointer. So never say by mistake that you are using auto pointers in your code. <http://www.cplusplus.com/reference/memory/auto_ptr/>
   2. **Unique Pointer `(Extremely Important)`** - <http://www.cplusplus.com/reference/memory/unique_ptr/>
   3. **Shared Pointer `(Extremely Important)`** - <http://www.cplusplus.com/reference/memory/shared_ptr/>
   4. **Weak Pointer** - <http://www.cplusplus.com/reference/memory/weak_ptr/>
5. **Chrono** - For performance analysis and tuning. Again this depends on the rt library and hence if you are using any feature of chrono then you must have to link the rt library with the code by add "-lrt" to your makefile for compilation.
<http://www.cplusplus.com/reference/chrono/>
6. **Miscellaneous** -
   1. Until C++11 by default the C++ compiler will provide 4 default functions to a class by default.
      1. Default Constructor.
      2. Destructor.
      3. Copy Constructor.
      4. Assignment Operator.
   2. Since C++11 the compiler will provide 2 more default functions along with the existing 4 default functions to any class by default.
      1. Default Constructor.
      2. Destructor.
      3. Copy Constructor.
      4. Assignment Operator. (Now called Copy Assignment Operator)
      5. Move Constructor. (Since C++11)
      6. Move Assignment Operator. (Since C++11)

I hope I have covered every important topic w.r.t. C++11 in this document.
Let me know if this helps.
