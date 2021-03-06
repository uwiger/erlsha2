
<h1>Module erlsha2</h1>

* [Description](#description)
* [Function Index](#index)
* [Function Details](#functions)


Implementations of SHA-224, SHA-256, SHA-384, SHA-512 in Erlang NIFs.



Copyright (c) 2009-2011 Stephen B. Vinoski, All rights reserved. Open source, BSD License

__Version:__ 2.0


__Introduced in:__ 03 Jan 2009


__Authors:__ Steve Vinoski ([`vinoski@ieee.org`](mailto:vinoski@ieee.org)) [_web site:_ `[http://steve.vinoski.net/](http://steve.vinoski.net/)`].

__References__* See [
the Secure Hash Standard](http://csrc.nist.gov/publications/fips/fips180-3/fips180-3_final.pdf) and the [Wikipedia SHA1
article](http://en.wikipedia.org/wiki/SHA1). Find the code [here](http://github.com/vinoski/erlsha2).


<h2><a name="index">Function Index</a></h2>



<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#sha224-1">sha224/1</a></td><td>Returns a SHA-224 hexadecimal digest.</td></tr></tr><tr><td valign="top"><a href="#sha224_init-0">sha224_init/0</a></td><td>Creates a SHA-224 context to be in subsequent calls to
sha224_update/2.</td></tr><tr><td valign="top"><a href="#sha224_update-2">sha224_update/2</a></td><td>Updates a SHA-224 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha224_final-1">sha224_final/1</a></td><td>Finishes the update of a SHA-224 Context and returns the computed
message digest.</td><tr><td valign="top"><a href="#sha256-1">sha256/1</a></td><td>Returns a SHA-256 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha256_init-0">sha256_init/0</a></td><td>Creates a SHA-256 context to be in subsequent calls to
sha256_update/2.</td></tr><tr><td valign="top"><a href="#sha256_update-2">sha256_update/2</a></td><td>Updates a SHA-256 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha256_final-1">sha256_final/1</a></td><td>Finishes the update of a SHA-256 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha384-1">sha384/1</a></td><td>Returns a SHA-384 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha384_init-0">sha384_init/0</a></td><td>Creates a SHA-384 context to be in subsequent calls to
sha384_update/2.</td></tr><tr><td valign="top"><a href="#sha384_update-2">sha384_update/2</a></td><td>Updates a SHA-384 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha384_final-1">sha384_final/1</a></td><td>Finishes the update of a SHA-384 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha512-1">sha512/1</a></td><td>Returns a SHA-512 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha512_init-0">sha512_init/0</a></td><td>Creates a SHA-512 context to be in subsequent calls to
sha512_update/2.</td></tr><tr><td valign="top"><a href="#sha512_update-2">sha512_update/2</a></td><td>Updates a SHA-512 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha512_final-1">sha512_final/1</a></td><td>Finishes the update of a SHA-512 Context and returns the computed
message digest.</td></tr></table>


<a name="functions"></a>


<h2>Function Details</h2>


<a name="sha224-1"></a>


<h3>sha224/1</h3>





<tt>sha224(M::message()) -> digest()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `digest() = binary()`




Returns a SHA-224 hexadecimal digest.




<h3>sha224_init/0</h3>





<tt>sha224_init() -> context()</tt><br/>* `context() = binary()`




Creates a SHA-224 context to be in subsequent calls to
sha224_update/2.




<h3>sha224_update/2</h3>





<tt>sha224_update(Context::context(), M::message()) -> newcontext()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `context() = binary()`<br/>
* `newcontext() = binary()`




Updates a SHA-224 context with message data and returns a new
context.




<h3>sha224_final/1</h3>





<tt>sha224_final(Context::context()) -> digest()</tt><br/>* `context() = binary()`<br/>
* `digest() = binary()`




Finishes the update of a SHA-224 Context and returns the computed
message digest.




<h3>sha256/1</h3>





<tt>sha256(M::message()) -> digest()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `digest() = binary()`




Returns a SHA-256 hexadecimal digest.




<h3>sha256_init/0</h3>





<tt>sha256_init() -> context()</tt><br/>* `context() = binary()`




Creates a SHA-256 context to be in subsequent calls to
sha256_update/2.




<h3>sha256_update/2</h3>





<tt>sha256_update(Context::context(), M::message()) -> newcontext()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `context() = binary()`<br/>
* `newcontext() = binary()`




Updates a SHA-256 context with message data and returns a new
context.




<h3>sha256_final/1</h3>





<tt>sha256_final(Context::context()) -> digest()</tt><br/>* `context() = binary()`<br/>
* `digest() = binary()`




Finishes the update of a SHA-256 Context and returns the computed
message digest.




<h3>sha384/1</h3>





<tt>sha384(M::message()) -> digest()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `digest() = binary()`




Returns a SHA-384 hexadecimal digest.
If the argument is a binary, the result is a binary, otherwise the




<h3>sha384_init/0</h3>





<tt>sha384_init() -> context()</tt><br/>* `context() = binary()`




Creates a SHA-384 context to be in subsequent calls to
sha384_update/2.




<h3>sha384_update/2</h3>





<tt>sha384_update(Context::context(), M::message()) -> newcontext()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `context() = binary()`<br/>
* `newcontext() = binary()`




Updates a SHA-384 context with message data and returns a new
context.




<h3>sha384_final/1</h3>





<tt>sha384_final(Context::context()) -> digest()</tt><br/>* `context() = binary()`<br/>
* `digest() = binary()`




Finishes the update of a SHA-384 Context and returns the computed
message digest.




<h3>sha512/1</h3>





<tt>sha512(M::message()) -> digest()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `digest() = binary()`




Returns a SHA-512 hexadecimal digest.




<h3>sha512_init/0</h3>





<tt>sha512_init() -> context()</tt><br/>* `context() = binary()`




Creates a SHA-512 context to be in subsequent calls to
sha512_update/2.




<h3>sha512_update/2</h3>





<tt>sha512_update(Context::context(), M::message()) -> newcontext()</tt><br/>* `message() = binary() | [iolist()](#type-iolist)`<br/>
* `context() = binary()`<br/>
* `newcontext() = binary()`<br/>




Updates a SHA-512 context with message data and returns a new
context.

<h3>sha512_final/1</h3>





<tt>sha512_final(Context::context()) -> digest()</tt><br/>* `context() = binary()`<br/>
* `digest() = binary()`




Finishes the update of a SHA-512 Context and returns the computed
message digest.



_Generated by EDoc, Mar 23 2011, 07:43:42._
