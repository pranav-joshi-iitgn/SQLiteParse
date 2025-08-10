This folder will contain the grammar of different queries. 

The grammar should be exactly the same as in the SQLite [documnetation](https://sqlite.org/lang.html).

Each file should have extension `.gram`

The file format is like this :

1. `#` for comments
2. A -> alpha for grammar rule, where alpha is an expression of terminals and non-terminals
3. All non-terminals must be in smaller case
4. Use single quotes to write terminals.
5. All tokens in a grammar rule must be space-separated.
6. Each file must have a list of non-terminals explained on the first line, such as `expr,column,table`, the url on the second line, the non-terminals used (imports) in 3rd line (with links to the `.gram` file explaining it) and then a blank line.
7. **Every grammar rule must lie fully on one line.**
8. There can be multiple rules for the same non-terminal's expansion. DO NOT write them using `|` . Instead, write all the rules on a new line, close to each other.
9. The non-terminal `C` reprsents "any character"
10. The non-terminal `A` represents "any alphabet"
11. The non-terminals `digit` and `hexdigit` represent the digits in base 10 and 16 .

## TODO

This is a to-do list of all non-terminals that need to be understood, along with the SQLite documentation page that they are found on.

[X] [literal](https://sqlite.org/syntax/literal-value.html)

