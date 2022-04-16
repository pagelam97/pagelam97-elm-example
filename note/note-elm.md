[all](https://package.elm-lang.org/packages/elm/core/latest/List#all) : (a -> [Bool](https://package.elm-lang.org/packages/elm/core/latest/Basics#Bool)) -> List a -> [Bool](https://package.elm-lang.org/packages/elm/core/latest/Basics#Bool)

Determine if all elements satisfy some test.测试是否全部元素通过函数，全部通过，返回true

```elm
all isEven [2,4] == True
all isEven [2,3] == False
all isEven [] == True
```



[any](https://package.elm-lang.org/packages/elm/core/latest/List#any) : (a -> [Bool](https://package.elm-lang.org/packages/elm/core/latest/Basics#Bool)) -> List a -> Bool

Determine if any elements satisfy some test.测试是否有元素通过测试，只要有一个通过测试返回Ture

```elm
any isEven [2,3] == True
any isEven [1,3] == False
any isEven [] == False
```
