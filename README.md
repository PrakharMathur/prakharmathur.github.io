# Learning advanced features introduced since C++11

Here is the list of items that have been introduced since C++11 and are frequently asked in Interviews of many Investment Banks, big software companies and start ups.

First follow this [link](http://www.codeproject.com/Articles/570638/Ten-Cplusplus-Features-Every-Cplusplus-Developer) to see some of the most important features that have been introduced as a part of C++11 and are frequently being used and being more precise must be used in all modern C++ applications.

Now following are the topics that you should prepare without fail.

1. **Move Semantics** - This is an important feature and you must understand how it works and why it is useful. Refer the links below.
   - <http://www.cprogramming.com/c++11/rvalue-references-and-move-semantics-in-c++11.html>
   - <http://stackoverflow.com/questions/3106110/what-are-move-semantics>
   - <http://www.codeproject.com/Articles/397492/Move-Semantics-and-Perfect-Forwarding-in-Cplusplus>
   - <https://en.cppreference.com/w/cpp/utility/move>
   - <http://www.cplusplus.com/reference/utility/move/?kw=move>
2. **New Containers**
   1. **Forward List**
      - <https://en.cppreference.com/w/cpp/container/forward_list>
      - <http://www.cplusplus.com/reference/forward_list/forward_list/>
   2. **Unordered Map** `(Extremly Important)`
      - <https://en.cppreference.com/w/cpp/container/unordered_map>
      - <http://www.cplusplus.com/reference/unordered_map/unordered_map/>
      - <http://stackoverflow.com/questions/21518704/how-does-c-stl-unordered-map-resolve-collisions>
      - <http://stackoverflow.com/questions/11337494/c-stl-unordered-map-implementation-reference-validity>
   3. **Unordered Multimap**
      - <https://en.cppreference.com/w/cpp/container/unordered_multimap>
      - <http://www.cplusplus.com/reference/unordered_map/unordered_multimap/>
   4. **Unordered Set**
      - <https://en.cppreference.com/w/cpp/container/unordered_set>
      - <http://www.cplusplus.com/reference/unordered_set/unordered_set/>
   5. **Unordered Multiset**
      - <https://en.cppreference.com/w/cpp/container/unordered_multiset>
      - <http://www.cplusplus.com/reference/unordered_set/unordered_set/>
   6. **Array**
      - <https://en.cppreference.com/w/cpp/container/array>
      - <http://www.cplusplus.com/reference/array/array/>
3. **Container Details** - Following page gives complete details of each container in a tabular format. Along with when the iterator is invalidated, which API each container supports, etc.
   - <https://en.cppreference.com/w/cpp/container>
4. **Multi Threading** `(Very Important)` - Always remember the C++11 Multi threading is just a OOPs based wrapper on pthread and is totally dependent on pthread library and hence you must have to link the pthread library with the code by adding "-lpthread" to your makefile for compilation. Please google to see how to use them as there are plenty of examples available. I will link my implementation of Ring Buffer code later which uses a lot of the C++11 features.
   1. **Atomic** `(Extremely Important)`
      - <https://en.cppreference.com/w/cpp/atomic/atomic>
      - <http://www.cplusplus.com/reference/atomic/>
   2. **Thread**
      - <https://en.cppreference.com/w/cpp/thread/thread>
      - <http://www.cplusplus.com/reference/thread/thread/>
   3. **Mutex**
      - <https://en.cppreference.com/w/cpp/thread/mutex>
      - <http://www.cplusplus.com/reference/mutex/>
   4. **Conditional Variable**
      - <https://en.cppreference.com/w/cpp/thread/condition_variable>
      - <http://www.cplusplus.com/reference/condition_variable/condition_variable/>
   5. **Thread Local Storage** `(Very Important)`
      - <https://en.cppreference.com/w/cpp/keyword/thread_local>
      - <http://en.cppreference.com/w/cpp/language/storage_duration>
5. **Smart Pointers** `(Extremely Important)` - You must understand clearly how these Smart Pointers are implemented internally. Refer this [link](http://www.codeproject.com/Articles/15351/Implementing-a-simple-smart-pointer-in-c). This implementation has few bugs but you will be able to understand the basic idea of how are they implemented and how they work.
   1. **Auto Pointer** `(Deprecated)`- Remember this is deprecated since C++11 and has been replaced with Unique Pointer. So never say by mistake that you are using auto pointers in your code.
      - <https://en.cppreference.com/w/cpp/memory/auto_ptr>
      - <http://www.cplusplus.com/reference/memory/auto_ptr/>
   2. **Unique Pointer** `(Extremely Important)`
      - <https://en.cppreference.com/w/cpp/memory/unique_ptr>
      - <http://www.cplusplus.com/reference/memory/unique_ptr/>
   3. **Shared Pointer** `(Extremely Important)`
      - <https://en.cppreference.com/w/cpp/memory/shared_ptr>
      - <http://www.cplusplus.com/reference/memory/shared_ptr/>
   4. **Weak Pointer**
      - <https://en.cppreference.com/w/cpp/memory/weak_ptr>
      - <http://www.cplusplus.com/reference/memory/weak_ptr/>
6. **Chrono** - For performance analysis and tuning. Again this depends on the rt library and hence if you are using any feature of chrono then you will have to link the rt library with the code by adding "-lrt" to your makefile for compilation.
   - <https://en.cppreference.com/w/cpp/header/chrono>
   - <http://www.cplusplus.com/reference/chrono/>
7. **Lambda Expressions**
   - <https://en.cppreference.com/w/cpp/language/lambda>
8. **Miscellaneous** -
   1. Until C++11 by default the C++ compiler provides 4 default functions to a class by default.
      1. Default Constructor.
      2. Destructor.
      3. Copy Constructor.
      4. Assignment Operator.
   2. Since C++11 the compiler provides 2 more default functions along with the existing 4 default functions to any class by default.
      1. Default Constructor.
      2. Destructor.
      3. Copy Constructor.
      4. Assignment Operator. (Now called Copy Assignment Operator)
      5. Move Constructor. (Since C++11)
      6. Move Assignment Operator. (Since C++11)

I hope I have covered every important topic w.r.t. C++11 in this document.
Let me know if this helps.

## About Author

### **_Prakhar Mathur_**

### LinkedIn - <https://www.linkedin.com/in/mathurprakhar>
