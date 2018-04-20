# Working with resources on statically-typed programming language

In *statically-typed* programming language, *compile* is required to make executable program.
Nowadays, practically compiling is usually carried out through *build* process because it sometimes requires fetching depenencies or a certain converting.
Statically-typed programming is better than dynamically-typed programming language at the point that various errors in your program would be detected by compilers' *type system*.

How many developers have suffured from writing SQL queries with raw string into their code ever on Earth?
Complicated texts like SQL queries should be written as a file instead of a string literal or a heredoc.

However, there is an issue that in case that a program dependents other static resources (e.g. text files, images, etc.), it ended up to get them through files and then it could not benefit by type-system.
Even though there are the same problem at dynamically-typed and it is not peculiar issue of statically-typed, it is unfortunate that the type-system could not be applied for various resources.

*Android Plugin*, used for building Android projects solves such issue at a high level. In an Android project, for instance, texts which would be shown in the app are stored all in one piece into a file named`string.xml` like following format:

```xml
<?xml version="1.0" encoding="utf-8"?>  
<resources>  
    <string name="hello">Hello World, MainActivity!</string>  
    <string name="app_name">HelloWorld</string>  
</resources>
```

```java
context.getString(R.string.hello);
```

then you can get them in Java code just like above, where `context` is a special variable in Android projects. It is convenience if such functionality is available and more versatile at non-Android projects as well. In this article, I am going to research how should such issue be solved at statically-typed programming languages, especially JVM languages.

## Use Cases

<em>WORK IN PROGRESS!</em>

- a single file to a single instance (e.g. SQL query file)
- a single file to a collection (e.g. `string.xml` in Android)
- many files to a big instance
- validate for several files

## References

- [maven-resources-plugin](https://github.com/apache/maven-plugins/tree/trunk/maven-resources-plugin)
