### Steps To Use This Template

- if you're not me, replace the license file with your desired license
- remove excess categories in .gitignore
- if working on a unity project set the unity yaml merge tool location in .gitconfig, otherwise remove it
- remove excess categories in .gitconfig
- adjust xml in Source/DefaultTemplate.csproj
- rename test, benchmarks, and main .csproj
- rename solution and reconnect projects to solution
- replace this readme

### Unity & Godot Game Engine Language Support

If you need to target both Unity and Godot I would currently reccomend netstandard 2.1 and C# 8, though Unity does not support *all* C# 8 language features.
Unity is working on switching to MSBuild but I wouldn't expect it any time soon.

| Engine Version    | .NET Version         | C# Version | Backend       | Build System   |
| ----------------- | -------------------- | ---------- | ------------- | -------------- |
| Unity 2018.1      | netstandard 2.0      | C# 7.3     | Mono or ILCPP | Unity Build    |
| Unity 2021.2      | netstandard 2.1      | C# 8.0     | Mono or ILCPP | Unity Build    |
| Unity 6           | netstandard 2.1      | C# 8.0     | Mono or ILCPP | Unity Build    |
| Godot 3.x         | .NET framework 4.7.2 | C# 7.3     | Mono          | MSBuild Roslyn |
| Godot 4.x Default | .NET 6               | C# 10      | CoreCLR       | MSBuild Roslyn |
| Godot 4.x Max     | .NET 8               | C# 12      | CoreCLR       | MSBuild Roslyn |

