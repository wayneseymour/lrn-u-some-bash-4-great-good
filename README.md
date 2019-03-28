# learn you some bash, for great good  :)

## create file backup using brace expansion

```
touch index.js
cp index.js{,.bak}
# => expands and executes, resulting in:
index.js index.js.bak
```

## generate dir structure using brace expansion

```
mkdir -p trepackages/{p1,p2,p3}/src
tree trepackages
trepackages
├── p1
│   └── src
├── p2
│   └── src
└── p3
    └── src
```

## var not defined, so provide a default

`echo ${str:-'my default'}`


## expand to last arg of previous command

```
touch README.md
vi !! 
# => Hit's return and then presents:
vi README.md
```


