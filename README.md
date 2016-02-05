This is a simple command line interface to the
[liquid library](http://liquidmarkup.org).

It takes variables on the command line in the form key=value, and processes
standard input using liquid with those variable substitutions. The resulting
output is printed to standard output.

For example, with the following command line:
```
./licmd n=4
```
and the following input:
```
{% for i in (1..n) %}{{n}}: repeat
{% endfor %}
```
we get the following output:
```
4: repeat
4: repeat
4: repeat
4: repeat

```
