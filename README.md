# Implementing a Key Value Database

Every key-value store (abbreviated to kv store) implements a get() and set() method that serve as its most important functionality. Like a Python dict, the kv store will set a value for some given key only if value is not None. However, the set() method should also function different from a Python dictionary by requiring the uniqueness of the key, that means if the key exists in the kv store, then throw a duplicate error.

For the get() method, we also want to replicate the same behavior from the Python dictionary. If we wish to get() the value for some given key, then we should get the saved value. However, if that key does not exist, the key-value store should throw an exception.

Remember to think about the API design as you develop the get() and set() methods. A handy class that you might want to use is the NodeKey class that we have implemented before. With this class, try to make it so the user of the kv store does not have to create a NodeKey objects first before calling set() on the kv store.
