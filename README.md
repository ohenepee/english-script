![ENGLISH SCRIPT](English script.png "ENGLISH SCRIPT")

This is English as a programming language.
The main purpose of this language is to make programming accessible to many more people, more fun and to facilitate programming computers via Voice.

Examples
--------
Here are some of our favorite examples from the tests, **working today**:

`beep three times`
(There will be a generation of programmers who will shake their heads that there ever was a programming language which did not interpret that sentence correctly.)

`square of 1,2 and 3 equals 1,4,9`

`add one to every odd number in 1,2,3 == 2,2,4`

`x is 2; if all 0,2,4 are smaller 5 then increase x; assert x equals 3 `

`beep every three seconds`

`counter is zero; repeat three times: add 1 to counter; done repeating; assert that the counter is 3`

`assert 3rd word in 'hi my friend' is 'friend'`

`last item in 'hi','you' is equal to 'you'`


```
While Peter is online on Skype
	make a beep
	sleep for 10 seconds
Done
```

```
How to check if someone is online on Skype
	Call java Skype.checkStaus(someone)
	Return yes If Result equals "online"
	Return no otherwise
Done
```

Language Specification
----------------------
Read the [DOSSIER](https://github.com/pannous/natural-english-script/tree/master/DOSSIER.md) for a more complete **language specification**, vision and some background. The grammar is not meant to be linguistically complete, but [functionality complete](https://en.wikipedia.org/wiki/Functional_completeness) and easily extendable. It is currently running in the [ruby](https://www.ruby-lang.org/en/) environment, but will soon compile to the [JVM](https://en.wikipedia.org/wiki/Java_Virtual_Machine) and as a final aim run natively.

To check out the current capabilities of this language have a look at the [tests](https://github.com/pannous/natural-english-script/tree/master/test/unit), at the [grammar](https://github.com/pannous/natural-english-script/blob/master/lib/english-script/english-parser.rb) and at the
[keywords](https://github.com/pannous/natural-english-script/blob/master/lib/english-script/english-tokens.rb)

EXPERIMENT
----------
Run it and see yourself!

`git clone git@github.com:pannous/english-script.git`
`./install.sh`

**experiment** by typing

`./english-script.sh 6 plus six`
`./english-script.sh "xs be 2,3,7,9; xs that are smaller than 7"`
`./english-script.sh examples/test.e`
`./english-script.sh` (no args for shell)
`english> 6 plus six`
`6`
`english>
`english> x is 2; if all 0,2,4 are smaller 5 then increase x`
`3`

Todos
-----
* Use the abstract syntax tree to compile instead of interpret (export via XML and Lisp s-expressions)
* Better (real) function argument matching: Integrate the sine curve in the interval 1 to 10 with step size .1
* Implement event system: Beep three times whenever the disc space is over 80%
* Hook into more existing libraries (java,ifttt,rubyosa?,...)
* IntelliJ plugin

Also check out cool similar projects:
[kal](https://github.com/rzimmerman/kal)
[dogescript](https://github.com/remixz/dogescript)

This language might soon be used in our successful beloved Jeannie assistant, which has over 4 million downloads so far:
http://www.voice-actions.com

For a background story/vision/philosophy/future of this project read the [DOSSIER](https://github.com/pannous/natural-english-script/tree/master/DOSSIER.md)

