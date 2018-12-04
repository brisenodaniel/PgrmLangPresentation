# Haskell Language and Lamba Calculus
What is Haskell?
* Completley functional language
* Static typing with type inference 
* Can do anything that an imperative language can do
    * But like any language, it's better at some things than others
* Absolutely nothing like you've ever seen before

## Types
As mentioned before, Haskell is  Statically typed like C++ or Java, but the way that types are used in Haskell is very different than in any C-ish language.

For example, here is a type declaration in C++ :

```c++ 
int num;
float num_2 = 9;
int *list = new int[30];

int squred (int a )
{
    return a*a;
}
```
In haskell, type declarations involve the `::` operator, which should be read as "is of type".

```haskell
num :: Int

num_2 = 9.0

list :: [Int]
list = []

squared :: Int -> Int
squared n = n*n
```
If functions are the heart of haskell, types are... the aorta? In any case, they are very very important. So important that in haskell they deserve their own line, and the typing system is more descriptive and important in Haskell than in imperative languages. To truly understand why, first we have to look at a function with multiple parameters.

```c++
float ave (float a, float b){
    return (float a + float b)/2;
}
```

```haskell
ave :: Float -> Float -> Float
ave a b = (a + b )/2
```
