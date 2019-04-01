# Sets


### 1. SADD

```
SADD key member[member...]

SADD myset "hello"

SADD myset "redis"

```

Add member into set stored


### 2. SMEMBERS 

```
SMEMBERS key 
```

Show all members of the set

### 3. SPOP 

```
spop key [count]
```

Removes and returns one or more random elements from the set value store at `key`.


### 4. SUNION 

```
SUNION key [key2...]

```
union of all the given sets, return all element into these set;
 
### SDIFF

```
SDIFF key1 key2 key3
```
第一个set中的差级， 返回第一个set 中其他不包括的元素

### 5. SDIFFSTORE

```
SDIFFSTORE key key1 key2
```
存储第一个 set的差级到 key中

### 6. SINTER 

```
SINTER key[key2]
```
intersection of all the sets;
交集


### 7. SCARD 

number of set (length)

### 8. SISMEMBER 

```
SISMEMBER key member

SISMEMBER myset "one"
```
if exist element in set return 1

if not exist element in set return 0

### 9. SREM 

```
SREM key member[member2...]
```

REMOVE, remove the specified members from the set at key

### 10.SUNIONSTORE

```
Sunionstore allset myset uset
```
store myset and uset all members into allset

