# Notes from Intro To DL

Dense layer: In each individual neuron in the dense layer takes the input data from all the other neurons before a currently existing one. [1]

![https://www.google.com/url?sa=i&url=https%3A%2F%2Fstackoverflow.com%2Fquestions%2F63675602%2Fhow-to-implement-a-neural-network-with-a-not-fully-connected-layer-as-the-final&psig=AOvVaw0f_kfcIkG7_tVJgRuygFhJ&ust=1708776495338000&source=images&cd=vfe&opi=89978449&ved=0CBUQjhxqFwoTCJC1itK2wYQDFQAAAAAdAAAAABAJ](image-1.png)

The Sequential Model [2]

Sequential model is used to stack plain layers arbitrarily. Each layer has exactly one input and output tensor.

A Sequential model is not appropriate when:

- Your model has multiple inputs or multiple outputs
- Any of your layers has multiple inputs or multiple outputs
- You need to do layer sharing
- You want non-linear topology (e.g. a residual connection, a multi-branch model)

By using SubClassing, we can define custom models, activation funcs etc. Also different network behaviours can be defined [example](../introtodeeplearning/lab1/Part1_TensorFlow.ipynb#C30:L6)


Resources

[1] https://www.educba.com/keras-dense/ \
[2] https://keras.io/guides/sequential_model/