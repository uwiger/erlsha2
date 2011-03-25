Module erlsha2
==============


<h1>Module erlsha2</h1>

* [Description](#description)
* [Function Index](#index)
* [Function Details](#functions)


Implementations of SHA-224, SHA-256, SHA-384, SHA-512 in Erlang NIFs.



Copyright (c) 2009-2011 Stephen B. Vinoski, All rights reserved. Open source, BSD License

__Version:__ 2.0


__Introduced in:__ 03 Jan 2009


__Authors:__ Steve Vinoski ([`vinoski@ieee.org`](mailto:vinoski@ieee.org)) (_web site:_ [`http://steve.vinoski.net/`](http://steve.vinoski.net/)).

__References__* See [
the Secure Hash Standard](http://csrc.nist.gov/publications/fips/fips180-3/fips180-3_final.pdf) and the [Wikipedia SHA1
article](http://en.wikipedia.org/wiki/SHA1). Find the code [here](http://github.com/vinoski/erlsha2).


<h2><a name="index">Function Index</a></h2>



<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#sha224-1">sha224/1</a></td><td>Returns a SHA-224 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha224_final-1">sha224_final/1</a></td><td>Finishes the update of a SHA-224 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha224_init-0">sha224_init/0</a></td><td>Creates a SHA-224 context to be in subsequent calls to
sha224_update/2.</td></tr><tr><td valign="top"><a href="#sha224_update-2">sha224_update/2</a></td><td>Updates a SHA-224 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha256-1">sha256/1</a></td><td>Returns a SHA-256 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha256_final-1">sha256_final/1</a></td><td>Finishes the update of a SHA-256 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha256_init-0">sha256_init/0</a></td><td>Creates a SHA-256 context to be in subsequent calls to
sha256_update/2.</td></tr><tr><td valign="top"><a href="#sha256_update-2">sha256_update/2</a></td><td>Updates a SHA-256 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha384-1">sha384/1</a></td><td>Returns a SHA-384 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha384_final-1">sha384_final/1</a></td><td>Finishes the update of a SHA-384 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha384_init-0">sha384_init/0</a></td><td>Creates a SHA-384 context to be in subsequent calls to
sha384_update/2.</td></tr><tr><td valign="top"><a href="#sha384_update-2">sha384_update/2</a></td><td>Updates a SHA-384 context with message data and returns a new
context.</td></tr><tr><td valign="top"><a href="#sha512-1">sha512/1</a></td><td>Returns a SHA-512 hexadecimal digest.</td></tr><tr><td valign="top"><a href="#sha512_final-1">sha512_final/1</a></td><td>Finishes the update of a SHA-512 Context and returns the computed
message digest.</td></tr><tr><td valign="top"><a href="#sha512_init-0">sha512_init/0</a></td><td>Creates a SHA-512 context to be in subsequent calls to
sha512_update/2.</td></tr><tr><td valign="top"><a href="#sha512_update-2">sha512_update/2</a></td><td>Updates a SHA-512 context with message data and returns a new
context.</td></tr></table>




<h2><a name="functions">Function Details</a></h2>


<a name="sha224-1"></a>

<h3>sha224/1</h3>






<pre>sha224(M :: <a href="#type-message">message()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Returns a SHA-224 hexadecimal digest.
<a name="sha224_final-1"></a>

<h3>sha224_final/1</h3>






<pre>sha224_final(Context :: <a href="#type-context">context()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Finishes the update of a SHA-224 Context and returns the computed
message digest.
<a name="sha224_init-0"></a>

<h3>sha224_init/0</h3>






<pre>sha224_init() -> <a href="#type-context">context()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li></ul>



Creates a SHA-224 context to be in subsequent calls to
sha224_update/2.
<a name="sha224_update-2"></a>

<h3>sha224_update/2</h3>






<pre>sha224_update(Context :: <a href="#type-context">context()</a>, M :: <a href="#type-message">message()</a>) ->
<a href="#type-newcontext">newcontext()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-newcontext">newcontext()</a> = binary()</pre></li></ul>



Updates a SHA-224 context with message data and returns a new
context.
<a name="sha256-1"></a>

<h3>sha256/1</h3>






<pre>sha256(M :: <a href="#type-message">message()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Returns a SHA-256 hexadecimal digest.
<a name="sha256_final-1"></a>

<h3>sha256_final/1</h3>






<pre>sha256_final(Context :: <a href="#type-context">context()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Finishes the update of a SHA-256 Context and returns the computed
message digest.
<a name="sha256_init-0"></a>

<h3>sha256_init/0</h3>






<pre>sha256_init() -> <a href="#type-context">context()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li></ul>



Creates a SHA-256 context to be in subsequent calls to
sha256_update/2.
<a name="sha256_update-2"></a>

<h3>sha256_update/2</h3>






<pre>sha256_update(Context :: <a href="#type-context">context()</a>, M :: <a href="#type-message">message()</a>) ->
<a href="#type-newcontext">newcontext()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-newcontext">newcontext()</a> = binary()</pre></li></ul>



Updates a SHA-256 context with message data and returns a new
context.
<a name="sha384-1"></a>

<h3>sha384/1</h3>






<pre>sha384(M :: <a href="#type-message">message()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Returns a SHA-384 hexadecimal digest.
If the argument is a binary, the result is a binary, otherwise the
<a name="sha384_final-1"></a>

<h3>sha384_final/1</h3>






<pre>sha384_final(Context :: <a href="#type-context">context()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Finishes the update of a SHA-384 Context and returns the computed
message digest.
<a name="sha384_init-0"></a>

<h3>sha384_init/0</h3>






<pre>sha384_init() -> <a href="#type-context">context()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li></ul>



Creates a SHA-384 context to be in subsequent calls to
sha384_update/2.
<a name="sha384_update-2"></a>

<h3>sha384_update/2</h3>






<pre>sha384_update(Context :: <a href="#type-context">context()</a>, M :: <a href="#type-message">message()</a>) ->
<a href="#type-newcontext">newcontext()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-newcontext">newcontext()</a> = binary()</pre></li></ul>



Updates a SHA-384 context with message data and returns a new
context.
<a name="sha512-1"></a>

<h3>sha512/1</h3>






<pre>sha512(M :: <a href="#type-message">message()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Returns a SHA-512 hexadecimal digest.
<a name="sha512_final-1"></a>

<h3>sha512_final/1</h3>






<pre>sha512_final(Context :: <a href="#type-context">context()</a>) -> <a href="#type-digest">digest()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-digest">digest()</a> = binary()</pre></li></ul>



Finishes the update of a SHA-512 Context and returns the computed
message digest.
<a name="sha512_init-0"></a>

<h3>sha512_init/0</h3>






<pre>sha512_init() -> <a href="#type-context">context()</a></pre>

<ul class="definitions"><li><pre><a name="type-context">context()</a> = binary()</pre></li></ul>



Creates a SHA-512 context to be in subsequent calls to
sha512_update/2.
<a name="sha512_update-2"></a>

<h3>sha512_update/2</h3>






<pre>sha512_update(Context :: <a href="#type-context">context()</a>, M :: <a href="#type-message">message()</a>) ->
<a href="#type-newcontext">newcontext()</a></pre>

<ul class="definitions"><li><pre><a name="type-message">message()</a> = binary() | iolist()</pre></li><li><pre><a name="type-context">context()</a> = binary()</pre></li><li><pre><a name="type-newcontext">newcontext()</a> = binary()</pre></li></ul>



Updates a SHA-512 context with message data and returns a new
context.


_Generated by EDoc, Mar 25 2011, 17:39:08._