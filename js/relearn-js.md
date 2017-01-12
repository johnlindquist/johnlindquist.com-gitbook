## Input and Output

Programming is taking data in and pushing a result out.

```javascript
4
```

If you push a `4` in, you get a `4` out.
<iframe
    frameborder="0"
    width="100%"
    height="163px"
    src="https://ramda-repl-hytrrglkax.now.sh/#?const%20numbers%20%3D%20%5B1%2C2%2C3%2C4%2C5%5D%0Afilter%28flip%28lt%29%284%29%29%28numbers%29%0A%20%20%20%20%20%20%0A%20%20%20%20"
>
</iframe>


## Comments

Add comments with `//` to explain what's going on in your code. Any text written on a line after the `//` will not be run by the computer. You can think of `//` as "meant for humans, not computers".

You read the first line.

Your computer will read "interpret" the second line.

```
//the number below is 4
4
```
<iframe
    frameborder="0"
    width="100%"
    height="163px"
    src="https://ramda-repl-hytrrglkax.now.sh/#?const%20numbers%20%3D%20%5B1%2C2%2C3%2C4%2C5%5D%0Amap%28multiply%282%29%29%28numbers%29%0A%20%20%20%20%20%20%0A%20%20%20%20"
>
</iframe>




## Functions

Before you write your own functions, start by using functions provided from [ramda](http://ramdajs.com/docs/).

The `inc` function increments a `Number` by 1 (that's a fancy way of saying "+ 1").

```
inc(4) //
```

<iframe
    frameborder="0"
    width="100%"
    height="163px"
    src="https://ramda-repl-hytrrglkax.now.sh/#?const%20names%20%3D%20%5B%22John%22%2C%20%22Mindy%22%2C%20%22Ben%22%5D%0Aconst%20prependName%20%3D%20curry%28%28last%2C%20first%29%3D%3E%20%60%24%7Bfirst%7D%20%24%7Blast%7D%60%29%0A%0Amap%28prependName%28%22Lindquist%22%29%29%28names%29%0A%20%20%20%20%20%20%0A%20%20%20%20%20%20%0A%20%20%20%20"
>
</iframe>







