## Angular compilation
    An Angular application consists largely of components and their HTML templates. Before the browser 
    can render the application, the components and templates must be converted to executable JavaScript 
    by an Angular compiler.

## Angular offers two ways to compile your application:

## 1.Just-in-Time (JIT) 
    which compiles your app in the browser at runtime

    JIT compilation is the default when you run the build-only or the build-and-serve-locally CLI commands:
> ng build
> ng serve
## 2.Ahead-of-Time (AOT)
    which compiles your app at build time.
    For AOT compilation, append the --aot flags to the build-only or the build-and-serve-locally CLI commands:
    ng build --aot
    ng serve --aot

## Why compile with AOT
    Faster rendering
    Fewer asynchronous requests
    Smaller Angular framework download size
    Detect template errors earlier
    Better security : AOT compiles HTML templates and components into JavaScript files long before 
    they are served to the client. 




