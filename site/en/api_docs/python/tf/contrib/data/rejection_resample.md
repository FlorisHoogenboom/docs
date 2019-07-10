page_type: reference
<style>{% include "site-assets/css/style.css" %}</style>

<!-- DO NOT EDIT! Automatically generated file. -->

# tf.contrib.data.rejection_resample

``` python
tf.contrib.data.rejection_resample(
    class_func,
    target_dist,
    initial_dist=None,
    seed=None
)
```



Defined in [`tensorflow/contrib/data/python/ops/resampling.py`](https://github.com/tensorflow/tensorflow/blob/r1.13/tensorflow/contrib/data/python/ops/resampling.py).

A transformation that resamples a dataset to achieve a target distribution. (deprecated)

Warning: THIS FUNCTION IS DEPRECATED. It will be removed in a future version.
Instructions for updating:
Use `tf.data.experimental.rejection_resample(...)`.

**NOTE** Resampling is performed via rejection sampling; some fraction
of the input values will be dropped.

#### Args:

* <b>`class_func`</b>: A function mapping an element of the input dataset to a scalar
    <a href="../../../tf/dtypes#int32"><code>tf.int32</code></a> tensor. Values should be in `[0, num_classes)`.
* <b>`target_dist`</b>: A floating point type tensor, shaped `[num_classes]`.
* <b>`initial_dist`</b>: (Optional.)  A floating point type tensor, shaped
    `[num_classes]`.  If not provided, the true class distribution is
    estimated live in a streaming fashion.
* <b>`seed`</b>: (Optional.) Python integer seed for the resampler.


#### Returns:

A `Dataset` transformation function, which can be passed to
<a href="../../../tf/data/Dataset#apply"><code>tf.data.Dataset.apply</code></a>.