## Dictionaries

The last built-in data structure is the dictionary which stores a map from one type of object (the key) to another (the value). The key must be an immutable type (string, number, or tuple). The value can be any Python data type.

Note: In the example below, the printed order of the keys returned by Python could be different than shown below. The reason is that unlike lists which have a fixed ordering, a dictionary is simply a hash table for which there is no fixed ordering of the keys (like HashMaps in Java). The order of the keys depends on how exactly the hashing algorithm maps keys to buckets, and will usually seem arbitrary. Your code should not rely on key ordering, and you should not be surprised if even a small modification to how your code uses a dictionary results in a new key ordering.

```python
>>> studentIds = {'jimbo': 42.0, 'jameson': 56.0, 'billy': 92.0 }
>>> studentIds['jameson']
56.0
>>> studentIds['billy'] = 'ninety-two'
>>> studentIds
{'jimbo': 42.0, 'jameson': 56.0, 'billy': 'ninety-two'}
>>> del studentIds['jimbo']
>>> studentIds
{'jameson': 56.0, 'billy': 'ninety-two'}
>>> studentIds['jimbo'] = [42.0,'forty-two']
>>> studentIds
{'jimbo': [42.0, 'forty-two'], 'jameson': 56.0, 'billy': 'ninety-two'}
>>> studentIds.keys()
['jimbo', 'jameson', 'billy']
>>> studentIds.values()
[[42.0, 'forty-two'], 56.0, 'ninety-two']
>>> studentIds.items()
[('jimbo',[42.0, 'forty-two']), ('jameson',56.0), ('billy','ninety-two')]
>>> len(studentIds)
3
```
