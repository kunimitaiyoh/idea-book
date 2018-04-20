# Working with resources on statically-typed programming language

In *statically-typed* programming language, *compile* is required to make executable program.
Nowadays, practically compiling is usually carried out through *build* process because it sometimes requires fetching depenencies or a certain converting.
Statically-typed programming is better than dynamically-typed programming language at the point that various errors in your program would be detected by compilers' *type system*.

However, there is an issue that in case that a program dependents other static resources (e.g. text files, images, etc.), it ended up to get them through files and then it could not benefit by type-system.
Even though there are the same problem at dynamically-typed and it is not peculiar issue of statically-typed, it is unfortunate that the type-system could not be applied for various resources.

*Android Plugin*, used for building Android projects solves such issue at high level.

## References

- [maven-resources-plugin](https://github.com/apache/maven-plugins/tree/trunk/maven-resources-plugin)
