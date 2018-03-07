# The Two programming language (Twolang)

Two is a new programming language developed in 2018 by Andrew Stuart.

Two's core rationale is to address the bloat of modern programming languages.

Modern programming languages are often feature heavy and as a result slow to run and carry the burden of many years of feature bloat.

You can think of Two as a "risc programming language" - one in which all the years of bloat and compatibility hacks have been peeled away to leave only the core value in place.

Two is Turing Complete, understandable for beginners and powerful enough to satisfy the most experienced developers.

As a new language, Two lacks the library support of its modern competitors but we expect this will come soon enough.

Two tends to referred to as Twolang because the author of the language wanted a cool name and felt one of the core words of the English language appropriate but failed to give much though to search engines and searchability so the cool and minimalist name 'Two' tends now to be a dorky and meaningless 'Twolang', but no matter what's done is done.

# Overview of Twolang.

The beauty and power of Twolang comes from it having only two 'instructions'.  But that's all any capable programmer needs.

# Two's first instruction is '0'.

# Two's second instruction is '1'.

It may take some time to fully understand the paradigm behind Two's programming model but once it clicks in you'll find it natural.

You write Twolang applications by tying together sequences of the Two instructions to formulate higher level constructs.

# Developing applications in Twolang

You can build any software application in Twolang given the two instructions available.  It is true that one of the down sides of Twolang applications can be a certain level of verbosity, but we believe that the tradeoff is worthwhile given the performance gains and code readaibility and maintainability which is easily on par with modern languages such as Perl.  

Here's an example to compare Hello World in Twolang with 'Hello World' in Perl (ref http://www.foo.be/docs/tpj/issues/vol4_3/tpj0403-0017.html):

Twolang example:
```
01010001111000101000111000001010101101001000101110001011010100010101100111100011110001
01000100000001011010011010011100101111100011 010001000000010 010001000000010
001111000011100 010001000000010010001000000010 010001000000010  010001000000010
010001000000010 010001000000010       010001000000010  010001000000010010001000000010
    010001000000010
    010001000000010
    010001000000010
```
Perl example:
```
sub ocr{@{$-[$@++]}=split$,for(split'\n',shift);for$@(0..4){for(0..51){++$_{$_
 }if($-[$@][$_]=~$")}}@&=(-1);for(sort{$a<=>$b}keys%_){push@&,$_ if($_{$_}>4)
  }push@&,52;for$@(0..13){@{$|[$@][$_]}=@{$-[$_]}[$&[$@]+1..$&[$@+1]-1]for(0..
   4)}for(@|){**=$_;$w=@{$*[$^=$$=0]}-1;for$@(0..4){for(1..$w){$^++if$*[$@][$_
    ]ne$*[$@][$_-1]}}for(0..$w){for$@(1..4){$$++ if$*[$@][$_]ne$*[$@-1][$_]}}
     for(0..20){push@},chr$_+65if(7*(8,4,2,9,2,3,7,8,1,$@,5,4,9,10,10,6,3,8,4,
      8,8)[$_]+(5,8,3,3,4,2,1,2,8,2,7,1,5,4,6,$@,3,6,8,4,1)[$_]==7*$^+$$)}}@}} 
```
# Twolang is whitespace sensitive

Twolang is whitespace sensitive.  Some feel that this is a detrimental decision for the language but others feel it improves readibility and consistency.

For example the Twolang authors considered that this code is far more understandable than the bracketed alternative below:

Figure 1:
```
010001000000010
    010001000000010
    010001000000010
```
Figure 2:
```
010001000000010: {
    010001000000010
    010001000000010
}
```
Whitespace is one of the many subtle but important decisions that pervade Twolang and are the outcome of many years research in programming language technology.   Clearly Figure 1 i the more readable and maintainable.

# Aliasing reference table for Twolang.

Keep this handy reference close when programming with Twolang:

```
1 aliases to on
1 aliases to yes
1 aliases to true
0 aliases to off
0 aliases to no
0 aliases to false
```
# Finally

This completes both the specification and tutorial of the Two programming language.

Check out and run some of the examples and we encourage you to build upon them and contribute back to the Twolang community.

# Appendix - implementations of Twolang in various languages:
One of the strengths of Twolang is that it can be easily implemented in a portable manner by many other higher level languages.

Ruby implementation of Twolang
```
(a = 1).to_s(2)     #=> "00001"
(a = 0).to_s(2)     #=> "00000"
```

Note that Python 2 and Python 3 are significantly different and porting of Twolang has been a major project recent completed.

```
Python 2.7.6 (v2.7.6:3a1db0d2747e, Nov 10 2013, 00:18:52)
Type "help", "copyright", "credits" or "license" for more information.
>>> b'0'
'0'
>>> b'1'
'1'
```

```
Python 3.5.2 (v3.5.2:4def2a2901a5, Jun 26 2016, 10:47:25)
Type "help", "copyright", "credits" or "license" for more information.
>>> b'0'
b'0'
>>> b'1'
b'1'
```

# The Tao of Twolang

"There's only Two ways to do it"

# Contributions

Pull requests are welcome.
