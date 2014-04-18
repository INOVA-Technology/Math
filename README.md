## It does your math homework!

Well a lot of it. Here's how you start it:

    ./solve

Then you may want to type help to see the available equations.

When you have the equation you want to use, type it at the prompt, followed by any arguments it requires. Example:

    > pythgrn-thrm-with-b-c 4 5
	3

Pretty simple right? It also has support for tab completion, so if you type `py` and then press tab, it'll finish it as `pythgrn-thrm-with-` and show you the options that you can finish it as.

# Using -l or --load

You can actually create a file with additional equations to load, and it very simple!

The format is like this:

    equation_name:var1, var2:(var1 + var2) ** 3
    second:variable:variable - 1

If you saved that to a file called equations, then just run `./solve -l equations`
Then you can use it like this:

    > equation_name 3 2
    125
	> second 9001
	9000
