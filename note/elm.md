### elm

## 介绍

## 基本类型、数据结构、自定义类型、类型别名

## 语法

## 例子

## 内置的一些函数

## 扩展







基本类型

- Bool
- String
- Char
- Float
- Int



- List      List String
- Tuples
- Records



自定义类型

```elm
type Player= teanA｜teamB String

--tag携带一个已知类型
```



类型别名

```elm
type alias Name=String

type alias Number=Int

type alias Player={name:Name, number:Number}



Player:Player
player={name="li",number:1}

setplayerNum:Int->Player->Player
setplayerNum 5 player=={player|number=5}

{-不使用类型别名
setplayerNum:Int->{name:Name, number:Number}->{name:Name, number:Number}
setplayerNum 5 player=={number|number=5}
-}
```



语法

- 函数

```elm
addfn:Int->Int->Int
addfn a b=a+b,
```

- 注释

```elm
--单行注释

{-多行注释-}

{--
addfn:Int->Int->Int
addfn a b=a+b,
--}
```

字符串拼接

```elm
toFullName person =
  person.firstName ++ " " ++ person.lastName

fullName =
  toFullName { fistName = "Hermann", lastName = "Hesse" }
```

条件语句

```elm
if weight > 90 then "fat"
else "Not very fat"
```

多分支的条件语句

 

```elm
 if year == 10 then      n + 1   
 
 else if key == 38 then      n - 1   
 
 else      n
```



case

```elm
update : Msg -> Model -> Model

update msg model =

  case msg of
  Increment ->
    model + 1

  Decrement ->
   model - 1
```

