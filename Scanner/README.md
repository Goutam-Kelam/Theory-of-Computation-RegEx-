In this exercise I was required to implement a DFA that recognizes the following tokens of a language:

	TOKEN     RECOGNIZES

	ID        Identifier defined as a sequence of alphanumerals including underscore that 
                 always begins with a letter or underscore

	NUM       Sequence of digits that does not contain redundant leading zeros

	PLUS      +
	MULT      *
	DIV       /
	SUB       -
	EXP       **
	MOD       %
	EQ        ==
	LT        <
	LPAREN    (
	RPAREN    )
	ASSIGN    =

The DFA implementation will receive a string, say, "a_1 = (b < 0) + 2 ** c / 6 $an assignment expression$", as input.
The expected output is:

ID ASSIGN LPAREN ID LT NUM RPAREN PLUS NUM POW ID DIV NUM

Note that anything specified within a pair of $'s is comment and so should be ignored while scanning the input.
Also the DFA should ignore white space while scanning the input. 
