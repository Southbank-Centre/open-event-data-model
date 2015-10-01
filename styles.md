---
layout: page
title: Styles
url: /docs/styles/
permalink: /docs/styles/

breadcrumb: Styles
---

<div class="panel panel-default">
  <div class="panel-body">
    Summary of the styles available in markdown, adapted from <a href="https://gist.github.com/jonschlinkert/5854601">this gist</a>.
  </div>
</div>

## Typography 

### Headings

Headings from `h1` through `h6` are constructed with a `#` for each level (note that they must be have an empty line after them):

{% highlight text %}
# h1 Heading

## h2 Heading

### h3 Heading

#### h4 Heading

##### h5 Heading

###### h6 Heading
{% endhighlight %}

Renders to:

# h1 Heading

## h2 Heading

### h3 Heading

#### h4 Heading

##### h5 Heading

###### h6 Heading

HTML:

{% highlight html %}
<h1>h1 Heading</h1>

<h2>h2 Heading</h2>

<h3>h3 Heading</h3>

<h4>h4 Heading</h4>

<h5>h5 Heading</h5>

<h6>h6 Heading</h6>
{% endhighlight %}

<br>
<br>
<br>


### Horizontal Rules

The HTML `<hr>` element is for creating a "thematic break" between paragraph-level elements. In markdown, you can create a `<hr>` with any of the following:

* `___`: three consecutive underscores
* `---`: three consecutive dashes
* `***`: three consecutive asterisks

renders to:

___

---

***


<br>
<br>
<br>


### Body Copy 

Body copy written as normal, plain text will be wrapped with `<p></p>` tags in the rendered HTML.

So this body copy:

{% highlight text %}
Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.
{% endhighlight %}
renders to this HTML:

{% highlight html %}
<p>Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.</p>
{% endhighlight %}


<br>
<br>
<br>


### Emphasis

#### Bold
For emphasizing a snippet of text with a heavier font-weight.

The following snippet of text is **rendered as bold text**.

{% highlight text %}
**rendered as bold text**
{% endhighlight %}
renders to:

**rendered as bold text**

and this HTML

{% highlight html %}
<strong>rendered as bold text</strong>
{% endhighlight %}

#### Italics
For emphasizing a snippet of text with italics.

The following snippet of text is _rendered as italicized text_.

{% highlight text %}
_rendered as italicized text_
{% endhighlight %}

renders to:

_rendered as italicized text_

and this HTML:

{% highlight html %}
<em>rendered as italicized text</em>
{% endhighlight %}

<br>
<br>
<br>


### Blockquotes
For quoting blocks of content from another source within your document.

Add `>` before any text you want to quote. 

{% highlight text %}
Add `>` before any text you want to quote. 
{% endhighlight %}

Renders to:

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.

and this HTML:

{% highlight html %}
<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
</blockquote>
{% endhighlight %}

Blockquotes can also be nested:

{% highlight text %}
> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. 
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi. 
>
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor 
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>>
>>> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. 
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi. 
{% endhighlight %}

Renders to:

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. 
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi. 
>
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor 
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
>>
>>> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue. 
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi. 


<br>
<br>
<br>


### Lists

#### Unordered
A list of items in which the order of the items does not explicitly matter.

You may use any of the following symbols to denote bullets for each list item:

{% highlight text %}
* valid bullet
- valid bullet
+ valid bullet
{% endhighlight %}

For example

{% highlight text %}
+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem
{% endhighlight %}

Renders to:

+ Lorem ipsum dolor sit amet
+ Consectetur adipiscing elit
+ Integer molestie lorem at massa
+ Facilisis in pretium nisl aliquet
+ Nulla volutpat aliquam velit
  - Phasellus iaculis neque
  - Purus sodales ultricies
  - Vestibulum laoreet porttitor sem
  - Ac tristique libero volutpat at
+ Faucibus porta lacus fringilla vel
+ Aenean sit amet erat nunc
+ Eget porttitor lorem

And this HTML

{% highlight html %}
<ul>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>
{% endhighlight %}

#### Ordered

A list of items in which the order of items does explicitly matter.

{% highlight text %}
1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
4. Facilisis in pretium nisl aliquet
5. Nulla volutpat aliquam velit
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem
{% endhighlight %}
Renders to:

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
4. Facilisis in pretium nisl aliquet
5. Nulla volutpat aliquam velit
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem

And this HTML:

{% highlight html %}
<ol>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit</li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ol>
{% endhighlight %}

**TIP**: If you just use `1.` for each number, GitHub will automatically number each item. For example:

{% highlight text %}
1. Lorem ipsum dolor sit amet
1. Consectetur adipiscing elit
1. Integer molestie lorem at massa
1. Facilisis in pretium nisl aliquet
1. Nulla volutpat aliquam velit
1. Faucibus porta lacus fringilla vel
1. Aenean sit amet erat nunc
1. Eget porttitor lorem
{% endhighlight %}

Renders to:

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
4. Facilisis in pretium nisl aliquet
5. Nulla volutpat aliquam velit
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem


<br>
<br>
<br>


### Code

#### Inline code
Wrap inline snippets of code with `` ` ``.

For example, `<section></section>` should be wrapped as "inline".

{% highlight html %}
For example, `<section></section>` should be wrapped as "inline".
{% endhighlight %}


#### Syntax highlighting and blocks of code

To activate syntax highlighting, simply add the file extension of the language you want to use directly to the highlight wrapper, and syntax highlighting will automatically be applied in the rendered HTML. For example, to apply syntax highlighting to JavaScript code:

<pre>{% raw  %}
{% highlight js %}
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
{% endhighlight %}
{% endraw %}</pre>

Renders to:

{% highlight js %}
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
{% endhighlight %}

And this complicated HTML:

{% highlight html %}
<code class="language-js" data-lang="js"><span class="nx">grunt</span><span class="p">.</span><span class="nx">initConfig</span><span class="p">({</span>
  <span class="nx">assemble</span><span class="o">:</span> <span class="p">{</span>
    <span class="nx">options</span><span class="o">:</span> <span class="p">{</span>
      <span class="nx">assets</span><span class="o">:</span> <span class="s1">'docs/assets'</span><span class="p">,</span>
      <span class="nx">data</span><span class="o">:</span> <span class="s1">'src/data/*.{json,yml}'</span><span class="p">,</span>
      <span class="nx">helpers</span><span class="o">:</span> <span class="s1">'src/custom-helpers.js'</span><span class="p">,</span>
      <span class="nx">partials</span><span class="o">:</span> <span class="p">[</span><span class="s1">'src/partials/**/*.{hbs,md}'</span><span class="p">]</span>
    <span class="p">},</span>
    <span class="nx">pages</span><span class="o">:</span> <span class="p">{</span>
      <span class="nx">options</span><span class="o">:</span> <span class="p">{</span>
        <span class="nx">layout</span><span class="o">:</span> <span class="s1">'default.hbs'</span>
      <span class="p">},</span>
      <span class="nx">files</span><span class="o">:</span> <span class="p">{</span>
        <span class="s1">'./'</span><span class="o">:</span> <span class="p">[</span><span class="s1">'src/templates/pages/index.hbs'</span><span class="p">]</span>
      <span class="p">}</span>
    <span class="p">}</span>
  <span class="p">}</span>
<span class="p">};</span></code>
{% endhighlight %}

<br>
<br>
<br>



### Tables
Tables are created by adding pipes as dividers between each cell, and by adding a line of dashes (also separated by bars) beneath the header. Note that the pipes do not need to be vertically aligned.


{% highlight text %}
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
{% endhighlight %}

Renders to:

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

And this HTML:

{% highlight html %}
<table>
  <tr>
    <th>Option</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>data</td>
    <td>path to data files to supply the data that will be passed into templates.</td>
  </tr>
  <tr>
    <td>engine</td>
    <td>engine to be used for processing templates. Handlebars is the default.</td>
  </tr>
  <tr>
    <td>ext</td>
    <td>extension to be used for dest files.</td>
  </tr>
</table>
{% endhighlight %}

#### Right aligned text

Adding a colon on the right side of the dashes below any heading will right align text for that column.

{% highlight text %}
| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
{% endhighlight %}

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |


<br>
<br>
<br>


### Links

#### Basic link

{% highlight text %}
[Assemble](http://assemble.io)
{% endhighlight %}

Renders to (hover over the link, there is no tooltip):

[Assemble](http://assemble.io)

HTML:

{% highlight html %}
<a href="http://assemble.io">Assemble</a>
{% endhighlight %}


#### Add a title

{% highlight text %}
[Upstage](https://github.com/upstage/ "Visit Upstage!")
{% endhighlight %}

Renders to (hover over the link, there should be a tooltip):

[Upstage](https://github.com/upstage/ "Visit Upstage!")

HTML:

{% highlight html %}
<a href="https://github.com/upstage/" title="Visit Upstage!">Upstage</a>
{% endhighlight %}

#### Named Anchors

Named anchors enable you to jump to the specified anchor point on the same page. For example, each of these chapters:

{% highlight text %}
# Table of Contents
  * [Chapter 1](#chapter-1)
  * [Chapter 2](#chapter-2)
  * [Chapter 3](#chapter-3)
{% endhighlight %}

will jump to these sections:

{% highlight text %}
## Chapter 1 <a id="chapter-1"></a>
Content for chapter one.

## Chapter 2 <a id="chapter-2"></a>
Content for chapter one.

## Chapter 3 <a id="chapter-3"></a>
Content for chapter one.
{% endhighlight %}

**NOTE** that specific placement of the anchor tag seems to be arbitrary. They are placed inline here since it seems to be unobtrusive, and it works.


<br>
<br>
<br>


### Images
Images have a similar syntax to links but include a preceding exclamation point.

{% highlight text %}
![Minion](http://octodex.github.com/images/minion.png)
{% endhighlight %}
![Minion](http://octodex.github.com/images/minion.png)

or
{% highlight text %}
![Alt text](http://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")
{% endhighlight %}
![Alt text](http://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

Like links, Images also have a footnote style syntax

{% highlight text %}
![Alt text][id]
{% endhighlight %}
![Alt text][id]

With a reference later in the document defining the URL location:

[id]: http://octodex.github.com/images/dojocat.jpg  "The Dojocat"


    [id]: http://octodex.github.com/images/dojocat.jpg  "The Dojocat"

