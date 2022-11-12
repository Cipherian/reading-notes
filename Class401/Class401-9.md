# Reading Notes 10/29/2022

## Dunder Methods

- In python special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognizze and end with double underscores.

- The dunder methods can replicate the behaviour of built in types. 

```Example
class LenSupport
def __len__(self):
  return str(self)
```

- the __getitem__ method which allows you to use python's slice syntax.
- ```obj[start:stop]```

- Special methods and the python data model. You can see python's data model asa powerful api you can interface with by implementing one or more dunder methods. If you want to write more pythonic code, knowing how to use dunder methods is important.

- __repr__ is the official string representation of an object

- __str__ is the unofficial string representation of an object

```EX: A method which iterates and adds transactions
def add_transaction(self, amount):
    if not isinstance(amount, int):
        raise ValueError('please use int for amount')
    self._transactions.append(amount)
```

```  EX2:
def balance(self):
    return self.amount + sum(self._transactions)
```

Source:[dbader](https://dbader.org/blog/python-dunder-methods)