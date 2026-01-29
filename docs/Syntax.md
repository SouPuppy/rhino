## Primitives

**Scalar Types**

- `i32` : 32-bit signed integer
- `u32` : 32-bit unsigned integer
- `f32` : IEEE 754 float type
- `bool` : Boolean type, either `true` or `false`
- `char` : Character type, default by 4bit-unicode

**Primitives Compound**

- Tensor `[][][]` : A tensor is an indexable multi-dimensional structure whose elements are of type `T`
- Tuples `( , )` : A collection of values of different types

**Derived Types**

While the language is defined by a minimal core of types, it also provides a set of built-in derived types for convenience and expressiveness.

- Set `{ }` : A set is defined by a collection of membership conditions over values of a single type `T`, determining whether a value belongs to the set.

    e.g.
    ```
    Set: Int {1, 2, x | x => x > 3}
    ```