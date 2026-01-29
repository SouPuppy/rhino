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

- Set `{ }` : A set is defined by a collection of membership condsitions over values of a single type `T`, determining whether a value belongs to the set.

    e.g.
    ```
    Set: Int {1, 2, x | x => x > 3}
    ```

## Types

Types are the essentials of this language, following the idea of type systeming, in here we have 3 ways to construct a type

- `type` : Type keyword is the most common way to derive types from existing ones:

    ```
    type <identifier> = {type constructor}
    ```

## Record & Struct

A record is a data value composed of several named fields grouped together as a single unit.
A `struct` is a language construct used to explicitly define and name a record type.

**A Record**

```
{
    x: i32;
    y: i32;
}
```

**A Structure**

```
struct Point {
    x: i32;
    y: i32;
}

p1: Point = {1, 2};
```