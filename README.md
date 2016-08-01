# x12lang (A Foo Lauguage)
A small programmig language with ANSI X12 syntax.

## Documentation

### Language basic
Every statement in X12Lang must have a '~' (tilde) as terminator
Statement must have a line terminator (\n, \r, \r\n)

### Source Structure
X12Lang source is divided into 3 sections.
* The first or the top section is reserved for library imports
* The second or middle section is variable declarations
* The third or final section is function commands

### Library Import (Does not currently do anything, nor does the libraries exist)
```
	ref stdio~ 
	ref stdlib~
```

### Variable Declaration
```
	nm1 msg : string~
	nm1 myInt : int~
	nm1 money : double~

	msg eq "hello world"~
	myInt eq 100~
	money eq 1.0~
```

### Function Commands (Currently only supports PRINT)
```
	prv "hello world"~
	prv msg~
	prv myInt~
	prv money~
	prv 123~
	prv "abc"~
	prv true~
```
