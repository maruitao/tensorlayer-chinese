API - 激活函数
==============================

为了尽可能地保持TensorLayer的简洁性，我们最小化激活函数的数量，因此我们鼓励用户直接使用
TensorFlow官方的函数，比如
``tf.nn.relu``, ``tf.nn.relu6``, ``tf.nn.elu``, ``tf.nn.softplus``,
``tf.nn.softsign`` 等等。更多TensorFlow官方激活函数请看
`这里 <https://www.tensorflow.org/versions/master/api_docs/python/nn.html#activation-functions>`_.


自定义激活函数
---------------------------

在TensorLayer中创造自定义激活函数非常简单。

下面的例子实现了把输入乘以2。对于更加复杂的激活函数，你需要用到TensorFlow的API。

.. code-block:: python

  def double_activation(x):
      return x * 2
      
      

.. automodule:: tensorlayer.activation

.. autosummary::

   identity
   ramp





激活函数 
---------------------

.. autofunction:: identity
.. autofunction:: ramp
