page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.contrib.graph_editor.get_name_scope_ops

``` python
tf.contrib.graph_editor.get_name_scope_ops(
    ops,
    scope
)
```



Defined in [`tensorflow/contrib/graph_editor/select.py`](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/graph_editor/select.py).

Get all the operations under the given scope path.

#### Args:

* <b>`ops`</b>: an object convertible to a list of tf.Operation.
* <b>`scope`</b>: a scope path.

#### Returns:

A list of tf.Operation.

#### Raises:

* <b>`TypeError`</b>: if ops cannot be converted to a list of tf.Operation.