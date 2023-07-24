Lens pattern is just a syntatical sugar for something like Haskell's lens.

## Single Updating Lens

```haskell
Lens a b = Functor f => (a -> f a) -> b -> f b
-- where a is the interested field and b is the outer structure

Predicate a = a -> Bool
```
Say we have:
<!-- a data structure `d`, and an interested field `f`, a lense `l` of type `Lens f d`, and a predicate `p` of type `` -->
```haskell
d :: D
f :: F
l :: Lens F D
p1 :: F -> Bool
p2 :: F -> Bool
```
Lens Pattern allow us to write this:
```python
d.f.p1.p2 = new_val

```
Which means: query field f of data structure d, if the predicate p1 and p2 are both true, then replace the value with new_val. Note that this only create a new data structure and binds it to d.

## Viewing

It's worth noting that, `f` doesn't have to be something that actually exists.
in the data structure, it may just be a `view` of underlying data structure. Nothing stops us from writing a slice lens:

For example, we may implement Bulk updating in a sequential container as this:

```haskell
slice :: Functor f => Range -> Lens (List a) (List a)
-- this is just a demonstration, not real code 
-- it doesn't type check but it won't harm for us to demonstrate how this works.
slice range f ds = 
  left, sliced, right = split_with_range ds range
  sliced_new = f sliced
  merge left sliced_new right
```

## Syntax

```ruby
a swap<- b, c # equivalent to `a = swap(a, b, c)`
a swap= b # equivalent to `a = swap(a, b)`
```