### Iterating a list/Array

Python:

```
nums = [1,2,3]
for num in nums:
   print (num)
for index, number in nums:
    print (index, number)
```

Java:

```
for (String element : array) {
    // Do something with element of type String
    System.out.println(element);
}

for (int i = 0; i < arr.length; i++) {
  System.out.println(i);
}
```

### Iterating through a range

Python:

```
# prints nums from 0 to n-1
for i in range(0,n):
   print i
   
# prints nums from n to 1:
for i in range(n, 0, -1):
   print i
```

Java:

```
```

### ascii to int, int to ascii

Python:

```
print (chr(97)) # prints 'a' since a => 97
print (ord('a')) # prints 97
```

Java
```
```

### Subarrays

Python
```
nums = [0,1,2,3,4,5]

nums[1:3]  # Prints [1,2]
nums[:3] # Prints [0,1,2]
nums[3:] # Prints [3,4,5]
```

### Data structures

#### List/ArrayList

pythom

```
a = [1,2,3]
b = [4,5]

c = a+b . # [1,2,3,4,5]
a.append(4) # a = [1,2,3,4]
a.pop()

a.sort()
a.sort(key = lambda num: num*2)
```

Java

```

public class IntervalComparator implements Comparator<Interval> {
    @Override
    public int compare(Interval i1, Interval i2) {
        return i1.start - i2.start;
    }
}

List<Interval> intervalList = Arrays.asList(intervals); // intervals - array
Collections.sort(intervalList, new IntervalComparator());

```

#### Dictionary/HashMap
Python 

```
#HashMap/Dictionary
dict = {'key1': 'val1', 'key2': 'val2'}
if 'key1' in dict:
   print 'true'
print dict.keys()
print dict.values()

for key,val in dict.items():
   print (key,val)
```

Java

```
```

#### Set/HashSet
Python

```
hashSet = set()
if item in hashSet: 
  print 'true'
h1 = set()
h2 = set()

print h1.intersection(h2)
h3 = h1.union(h2)
```

Java
```
```

#### Heap/PriorityQueue
Python 
```
endTimeQueue = Q.PriorityQueue()
endTimeQueue.put(intervals[0].end)
endTimeQueue.get()   // This will remove the least element
earliestEndTimeClassroom = endTimeQueue.queue[0] 
```

Java
```
PriorityQueue<Integer> endTimeClassRoomQueue = new PriorityQueue(intervals.length);
endTimeClassRoomQueue.add(intervals[0].end);
int leastStartTimeClassroom = endTimeClassRoomQueue.peek(); 
endTimeClassRoomQueue.poll();

```
#### OrderedDictionary

