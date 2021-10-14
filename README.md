# SkiaSharpPackError

Demonstration of a SkiaSharp pack error

To reproduce the error execute the following command in the project folder:

```shell
msbuild SkiaSharpAppiOS/ClassLibraryiOS/ClassLibraryiOS.csproj -restore -t:pack
```

Gives the following error:

```shell
".../SkiaSharpAppiOS/SkiaSharpAppiOS/ClassLibraryiOS/ClassLibraryiOS.csproj" (pack target) (1) ->
(GenerateNuspec target) -> 
  .../.nuget/packages/nuget.build.tasks.pack/5.6.0/build/NuGet.Build.Tasks.Pack.targets(198,5): error : 
  The file '.../SkiaSharpAppiOS/SkiaSharpAppiOS/ClassLibraryiOS/bin/iPhoneSimulator/Debug/Native.ClassLibraryiOS.manifest' to be packed was not found on disk. 
  [.../SkiaSharpAppiOS/SkiaSharpAppiOS/ClassLibraryiOS/ClassLibraryiOS.csproj]
```
