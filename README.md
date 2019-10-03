### defrom
---
https://github.com/Pylons/deform


```py
// deform/tests/test_schema.py
import unittest

def invalid_exc(func, *arg, **kw):
  from colander import Invalid
  
  try:
    func(*arg, **kw)
  except Invalid as e:
    return e
  else:
    raise AssertionError("Invalid not raised")
    
class TestFileData(unittest.TestCase):
  def _makeOne(self):
    from deform.schema import FileData
    
    return FileData()
    
  def test_deserialize_nul(self):
    from colander import null
    
    typ = self._makeOne()
    node = DummySchemaNode()
    result = typ.deserialize(node, null)
    self.assertEqual(result, null)
  
  def test_deserialize_not_null(self):
  
  
  def test_deserialize_not_null(self):
  
  
  
  def test_serialize_no_uid(self):


```

```
```

```
```

