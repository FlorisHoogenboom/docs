page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.contrib.learn.InputFnOps

## Class `InputFnOps`





Defined in [`tensorflow/contrib/learn/python/learn/utils/input_fn_utils.py`](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/learn/python/learn/utils/input_fn_utils.py).

A return type for an input_fn (deprecated).

THIS CLASS IS DEPRECATED. Please use tf.estimator.export.ServingInputReceiver
instead.

This return type is currently only supported for serving input_fn.
Training and eval input_fn should return a `(features, labels)` tuple.

The expected return values are:
  features: A dict of string to `Tensor` or `SparseTensor`, specifying the
    features to be passed to the model.
  labels: A `Tensor`, `SparseTensor`, or a dict of string to `Tensor` or
    `SparseTensor`, specifying labels for training or eval. For serving, set
    `labels` to `None`.
  default_inputs: a dict of string to `Tensor` or `SparseTensor`, specifying
    the input placeholders (if any) that this input_fn expects to be fed.
    Typically, this is used by a serving input_fn, which expects to be fed
    serialized `tf.Example` protos.

<h2 id="__new__"><code>__new__</code></h2>

``` python
__new__(
    _cls,
    features,
    labels,
    default_inputs
)
```

Create new instance of InputFnOps(features, labels, default_inputs)



## Properties

<h3 id="features"><code>features</code></h3>



<h3 id="labels"><code>labels</code></h3>



<h3 id="default_inputs"><code>default_inputs</code></h3>




