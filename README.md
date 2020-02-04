# MveFuncBuild
minimum viable example of function


## build 

1. clone
2. Open in visual studio
3. build

no folder name `http` recreated and foøe `function.json` is then also missing

## Debug

1. clone
2. open in visual studio
3. run

no functions available.

## cmd line build

```sh
dotnet build .\FunctionV3.sln
```

Some warnings, no folders available.


## manual fix

do the following from root folder

1. `dotnet build .\FunctionV3.sln`
2. ` mkdir .\FunctionV3\bin\Debug\netcoreapp3.1\http`
3. `copy .\FunctionV3\http\function.json .\FunctionV3\bin\Debug\netcoreapp3.1\http\`
4. `cd .\FunctionV3\bin\Debug\netcoreapp3.1`
5. `func start`

now it works as expected
