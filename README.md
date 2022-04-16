# RBtree
A Red Black Tree template in C++ 98

using ft namespace:

ft::RBtree<KEY, VALUE>

Key must be a type which is compareable with > < == !=.


# Types:
valPtr  is a pointer to the data, pair(KEY, VALUE)
- valPtr->first   ==  KEY
- calPtr->second  ==  VALUE


# Public member functions:

bool    empty()
- returns true if tree is empty, flase if not


size_type size()
- returns size of tree, usually size_type is size_t


void    clear()
- deletes and frees all data in the tree


bool    find(KEY key)
- return true if key already in the tree, false if not


valPtr  getValue(KEY key)
- NULL if key was not found
- valPtr to the found data


void    setValue(KEY key, VALUE val)
- changes value of key if key was found
- inserts a new element key with val if key was not found


void    erase(valPtr data)
- deletes the element from the tree if key was found


void    erase(KEY key, VALUE val)
- overload for separated arguments key and val


void    insert(KEY key, VALUE val)
- inserts a new element in the tree
- does nothing if key is present already


void    print()
- prints out the tree in std::out

