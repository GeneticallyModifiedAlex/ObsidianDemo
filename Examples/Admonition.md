#plugin #Examples #guide
[Official Documentation](https://github.com/valentine195/obsidian-admonition)

[microsoft syntax](https://docs.microsoft.com/en-us/contribute/markdown-reference)
```text
ad-name
```

Custom Types
```ad-note
icon: google 
title:Custom note
color: 100,220,100

You can make your own custom notes
```
Standard types:
```ad-note
icon: triforce

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla.

```

```ad-abstract

ad-abstract

```

```ad-tip

```

```ad-example

```

```ad-question

```

```ad-info

```

```ad-danger

```

```ad-success

```

```ad-warning

```

```ad-quote

```

```ad-failure

```
---
#Admonition #Guide #Examples 

`````ad-note
title: Nested Admonitions
collapse: open

Hello! #nested

````ad-note
title: This admonition is nested.
This is a nested admonition!

```ad-warning
title: This admonition is closed.
collapse: close
```

````

This is in the original admonition.
`````
````ad-info
#Admonittion #codeblock #nested
```ad-bug
title: I'm Nested!
~~~javascript
throw new Error("Oops, I'm a bug.");
~~~
```

```javascript
console.log("Hello!");
```

````


