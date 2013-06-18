---
layout: post
title: "Racket 101"
date: 2013-06-18 09:51
comments: true
categories: [racket, programming]
published: false
---

This is a brief introduction to Racket that I'm writing as I learn it.

http://imgs.xkcd.com/comics/lisp.jpg
{% img http://imgs.xkcd.com/comics/lisp.jpg %}

What is Racket?
---------------

This might seem like an odd question to address in a tutorial since if you're reading this you must have already decided that you want to learn Racket so you must already have an idea what it is. But...

``` racket Language declaration
#lang racket
```

Racket requries a language declaration. Racket supports multiple languages? Macros blah. Don't need to be lisp-like. Desktop of tools. Racket is a set of tools - not quite. Desktop has powerpoint, but can't change it easily.  Desktop of tools to write programs.  Everything is a program. Programmer wants to write programs to do things.

Wishes. Allows multiple languages. A language that lets you write programming languages.

* everything is a program
* Concpets are constructs in the programming language
* programming language is extensible

Pictures are values.


Different langs:

Can choose how file is parsed.  Not all languages support swithing languages within the stream.

*links?*
* racket
* roman numeral - macro extension, pattern matching macro
* racket/class - starts with racket and adds class syntax (implemented as a library)
* bsl - almost the same but (1 + 2) has a better error message
* typed/racket - adds static types
* scribble - for writing docs, mostly write in prose
* honu - javascript syntax
* frtime - async programming signalling


Define
------

'+' is a function
Function call '(' + name of function + arguments +')'

``` racket 3 versions of cube verbatim from pl
(define x 3)

(define cube1
	(lambda (x)
		(* x (* x x))))

(define cube2
	(lambda (x)
		(* x x x)))		

;syntactic sugar
(define (cube2 x)	
	(* x x x))
```

Racket Constructs
-----------------

[] is the same as () - easy to turn syntax into a syntax tree (parsing)

### Term

* primitive atom #t, #f, 2, "Foo" x
* special form define, lambda, if - body has runes specific to the special form.
* sequence of terms (t1 t2 t3 ... tn) is this where 'list' in lisp comes from?
	* if t1 
	* if t1 is not special form or atom then it is a function call


Dr

Hello World (and others) in Racket  
----------------------------------

``` racket Expressions
	"Hello World"

	(+ 1 2)

	(* 3 4)

	(+ 1 (* 3 2))

	(define (some-foo x)
	  (* 3 x))
```


* dialect of List, descant of scheme - links
* DrRacket





Foo bar

* foo
* bar

