

# Module marina_buffer #
* [Data Types](#types)
* [Function Index](#index)
* [Function Details](#functions)

<a name="types"></a>

## Data Types ##




### <a name="type-buffer">buffer()</a> ###


<pre><code>
buffer() = #buffer{buffered = iolist(), current = non_neg_integer(), pending = non_neg_integer() | undefined}
</code></pre>




### <a name="type-frame">frame()</a> ###


<pre><code>
frame() = #frame{flags = 0 | 1, stream = integer(), opcode = non_neg_integer(), body = iolist() | binary()}
</code></pre>

<a name="index"></a>

## Function Index ##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#decode-2">decode/2</a></td><td></td></tr><tr><td valign="top"><a href="#new-0">new/0</a></td><td></td></tr></table>


<a name="functions"></a>

## Function Details ##

<a name="decode-2"></a>

### decode/2 ###

<pre><code>
decode(Data::binary(), Buffer::<a href="#type-buffer">buffer()</a>) -&gt; {[<a href="#type-frame">frame()</a>], <a href="#type-buffer">buffer()</a>}
</code></pre>
<br />

<a name="new-0"></a>

### new/0 ###

<pre><code>
new() -&gt; <a href="#type-buffer">buffer()</a>
</code></pre>
<br />

