# Cooperative distributed kill with asymmetric behavior using C++ concurrent programming
Using the deferred option of std::sync allows us to delay the execution of the controller task until we receive input indicating a key has been hit. 
This eliminates the need for condition variables, mutexes, and other synchronization mechanisms in the controller task.
# Note
Multiple threads can call std::future::wait() on the same std::future object without any issues. The std::future is a thread-safe class, and its member functions can be called by multiple threads concurrently.
