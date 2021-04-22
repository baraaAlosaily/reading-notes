# ERRORS AND DEBIGGING

![error](https://www.elegantthemes.com/blog/wp-content/uploads/2018/02/502-error.png)

JavaScript can be hard to learn and everyone makes mistakes when writing it. This chapter will help you learn how to find the errors in your code. It will also teach you how to write scripts that deal with potential errors gracefully.

When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser gives look cryptic at fi rst, but they can help you determine what went wrong in your JavaScript and how to fix it. In this note you will learn about:

1. THE CONSOLE & DEV TOOLS: Tools built into the browser that help you hunt for errors.
2. COMMON PROBLEMS: Common sources of errors, and how to solve them.
3. HANDLING ERRORS How code can deal with potential errors gracefully.

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:

![run](./img/run.png)

### EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.

EXECUTION CONTEXT
Every statement in a script lives in one of three
execution contexts:

1. GLOBAL CONTEXT
   Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT
   Code that is being run within a function.
   Each function has its own function context.
3. EVAL CONTEXT (NOT SHOWN)
   Text is executed like code in an internal function
   called eva l {) (which is not covered in this book).

## EXECUTION CONTEXT & HOISTING

![hos](./img/hos.png)

## UNDERSTANDING SCOPE

In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

![new](./img/new.png)

## UNDERSTANDING ERRORS

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.

![err](./img/err.png)

## How to Debug JavaScript Errors

Debugging JavaScript errors in a production environment can be a difficult experience. More often than not, the error reports are vague, and identifying the underlying causes can be difficult at best. That said, there are a few common steps that can be followed towards identifying and resolving errors that crop up in production.

### Gathering information

Step 1: Attempt to replicate circumstances
In software development, the first step towards debugging any issue is attempting to replicate the circumstances. With most programming languages, this is bolstered by reviewing logs leading up to an error, but with client-side JavaScript, this type of diagnosis requires significantly more foresight (more on that below).

###Before we can replicate any circumstances of an issue, and assuming we have access to any production logs, we first need to establish some testing guidelines. This involves doing things like mimicking the production database, the user accounts involved, and even the operating system. Everything is fair game here.

### Step 2: Test assumptions

Once you've established the circumstances that you think might throw the exception or error you are hunting down, it's time to test them. Never test exceptions in production. Development and staging environments are designed to be breakable without any impact on the end users, so always always always try to break your code in a safe environment.

### Step 3: Increase logging

More information is always better. Using the methods described in Where are JavaScript Errors Logged?, the first step towards diagnosing any issue is to increase the amount of data you are logging. This allows you to see everything that is happening before and after a problem occurs. There is a good chance that the problems you are experiencing have potential warnings associated with them that don't necessarily make it into the logs by default.

### Step 4: Adjust test parameters and try again

If you were unable to replicate the problem in Step 2, then it's back to the drawing board. Not every error is easy to reproduce, and may have time-based constraints or something else making it difficult to replicate in a non-production environment. Jump back to Step 1, adjust your test parameters, and try it all over again.

### What are Source Maps?

In a production environment, JavaScript files are often compressed. While this is a great way to speed up any application, it can make debugging a nightmare, as the files you are trying to debug are practically unreadable. This is where source maps come into the picture. Supported by most modern browsers, a source map is a file that maps uncompressed code to compressed code, allowing you to see exactly what is going on within a production environment.

While most minification tools have built-in support for source maps, it is important to understand exactly how the browser connects compressed code to uncompressed code. In a nutshell, this comes in the form of a comment within a compressed JavaScript file that points directly to the source map.

`//# sourceMappingURL=http://example.com/path/to/your sourcemap.map`

As an example, let’s take a look at the developer console without source maps enabled. In particular, do you see how the source file says "Generated by CoffeeScript" and there is automatically generated JavaScript below?

![iii](https://images.ctfassets.net/cj4mgtttlyx7/6QQ93ce9hqvRchGuvuOA16/e7073f9f4ac0e38bcbbf8c8e00c0cc93/image_0.png)

Developer Console Debugger
While the production JavaScript file can be viewed and debugged it's not the code I wrote. The original source file is written in CoffeeScript, which means that any insight gleaned from the compiled code will have to be translated back into the original source file.
Now, let’s take a look at the same example with source maps enabled:

![ooo](https://images.ctfassets.net/cj4mgtttlyx7/3KHvLowUOUVlczBwnEDE5k/cf2ad129d8e990434349dee33b0f6cfa/image_1.png)

Developer Console Debugger
With source maps enabled, the breakpoint in the compiled script can be mapped directly to the original source file in CoffeeScript. This makes it possible to debug issues in the context of the source files, rather than the compiled and sanitized files that make it into the production environment.
