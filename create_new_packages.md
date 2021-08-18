[PkgTemplates.jl](https://github.com/invenia/PkgTemplates.jl) is very handy to create new packages from scratches, for example

```julia
using PkgTemplates
t = Template(;
    user = "lucaferranti",
    authors = "Luca Ferranti et al.",
    julia = VERSION,
    plugins = [
        Git(),
        GitHubActions(; x86 = true, windows=true, osx=true),
        Codecov(),
        Documenter{GitHubActions}(),
    ],
)
```

after that you can create the package with

```julia
t("MyPkgName")
```