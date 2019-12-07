#Learning Advanced C++
Here is the list of items that have been introduced in C++11 and are frequently asked in Interviews of many Investment Banks.

First follow this link to see some of the most important features that have been introduced as a part of C++11 and are frequently being used and being more precise must be used in all modern C++ applications.

http://www.codeproject.com/Articles/570638/Ten-Cplusplus-Features-Every-Cplusplus-Developer

Now are following are the topics that you should prepare without fail.
1. Move Semantics - This is an important feature and you must understand how it works and why it is useful. Refer the links below.
-http://www.cprogramming.com/c++11/rvalue-references-and-move-semantics-in-c++11.html
-http://stackoverflow.com/questions/3106110/what-are-move-semantics
-http://www.codeproject.com/Articles/397492/Move-Semantics-and-Perfect-Forwarding-in-Cplusplus
-http://www.cplusplus.com/reference/utility/move/?kw=move
2. New Data Structures
   i. Forward List - http://www.cplusplus.com/reference/forward_list/forward_list/
   ii. Unordered Map(Extremly Important),Set, Multimap - http://www.cplusplus.com/reference/unordered_map/unordered_map/
http://stackoverflow.com/questions/21518704/how-does-c-stl-unordered-map-resolve-collisions
http://stackoverflow.com/questions/11337494/c-stl-unordered-map-implementation-reference-validity
   iii. Array - http://www.cplusplus.com/reference/array/array/
3. Multi Threading(very Important) - Always remember the C++11 Multi threading is just a OOPs based wrapper on pthread and is totally dependent on pthread library and hence you must have to link the pthread library with the code by add "-lpthread" to your makefile for compilation. Please google to see how to use them as there are plenty of examples available. I will send a my implementation of Ring Buffer code later which uses a lot of the C++11 features.
   i. Atomic(Extremely Important) - http://www.cplusplus.com/reference/atomic/
   ii. Thread - http://www.cplusplus.com/reference/thread/thread/
   iii. Mutex - http://www.cplusplus.com/reference/mutex/
   iv. Conditional Variable - http://www.cplusplus.com/reference/condition_variable/condition_variable/
   v. Thread Local Storage(Very Important) - http://en.cppreference.com/w/cpp/language/storage_duration
4. Smart Pointers (Extremely Important) - You must understand clearly how these Smart Pointers are implemented internally. Refer this link. This implementation has few bugs but you will be able to understand the basic idea of how are they implemented and how they work.
http://www.codeproject.com/Articles/15351/Implementing-a-simple-smart-pointer-in-c .
   i. Auto Pointer - Remember this is deprecated in C++11 and have been replaced with Unique Pointer. So never say by mistake that you are using auto pointers in your code. http://www.cplusplus.com/reference/memory/auto_ptr/
   ii. Unique Pointer(Extremely Important) - http://www.cplusplus.com/reference/memory/unique_ptr/
   iii. Shared Pointer(Extremely Important) - http://www.cplusplus.com/reference/memory/shared_ptr/
   iv. Weak Pointer - http://www.cplusplus.com/reference/memory/weak_ptr/
5. Chrono - For performance analysis and tuning. Again this depends on the rt library and hence if you are using any feature of chrono then you must have to link the rt library with the code by add "-lrt" to your makefile for compilation.
http://www.cplusplus.com/reference/chrono/
6. Miscellaneous -
   i. Until C++11 by default the C++ compiler will provide 4 default functions to a class by default.
  	a. Default Constructor.
  	b. Destructor.
  	c. Copy Constructor.
  	d. Assignment Operator.
   ii. Since C++11 the compiler will provide 2 more default functions along with the existing 4 default functions to any class by default.
  	a. Default Constructor.
  	b. Destructor.
  	c. Copy Constructor.
  	d. Assignment Operator. (Now called Copy Assignment Operator)
	e. Move Constructor. (Since C++11)
  	f. Move Assignment Operator. (Since C++11)

I hope I have covered every important topic w.r.t. C++11 in this document.
Let me know if this helps.
