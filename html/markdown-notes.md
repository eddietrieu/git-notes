# plugins

```
r1 = f.a("vendor/markdown-it-mark.js","module");`
```
---
```
if (n.use(r1), e.taskList) {
  var i = f.a("vendor/markdown-it-task-lists.js", "module");
  n.use(i)
}
```

a~~nnie~~

---

# h1 Heading 8-)
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading


## Horizontal Rules

___

---

***


## Typographic replacements

Enable typographer option to see result.

(c) (C) (r) (R) (tm) (TM) (p) (P) +-

test.. test... test..... test?..... test!....

!!!!!! ???? ,,  -- ---

"Smartypants, double quotes" and 'single quotes'


## Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Strikethrough~~


## Blockquotes

> this is a regular blockquote

> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.



## Lists

Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa


1. You can use sequential numbers...
1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar


## Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting

``` js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

## Tables

| Option | Description                                                               |
| ------ | ------------------------------------------------------------------------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default.    |
| ext    | extension to be used for dest files.                                      |

Right aligned columns

| Option | Description                                                               |
| -----: | ------------------------------------------------------------------------: |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default.    |
| ext    | extension to be used for dest files.                                      |


## Links

[link text](http://dev.nodeca.com)

[link with title](http://nodeca.github.io/pica/demo/ "title text!")

Autoconverted link https://github.com/nodeca/pica (enable linkify to see)


## Images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

Like links, Images also have a footnote style syntax

![Alt text][id]

With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"


## Plugins

The killer feature of `markdown-it` is very effective support of
[syntax plugins](https://www.npmjs.org/browse/keyword/markdown-it-plugin).


### [Emojies](https://github.com/markdown-it/markdown-it-emoji)

> Classic markup: :wink: :crush: :cry: :tear: :laughing: :yum:
>
> Shortcuts (emoticons): :-) :-( 8-) ;)

see [how to change output](https://github.com/markdown-it/markdown-it-emoji#change-output) with twemoji.


### [Subscript](https://github.com/markdown-it/markdown-it-sub) / [Superscript](https://github.com/markdown-it/markdown-it-sup)

- 19^th^
- H~2~O


### [\<ins>](https://github.com/markdown-it/markdown-it-ins)

++Inserted text++


### [\<mark>](https://github.com/markdown-it/markdown-it-mark)

==Marked text==


### [Footnotes](https://github.com/markdown-it/markdown-it-footnote)

Footnote 1 link[^first].

Footnote 2 link[^second].

Inline footnote^[Text of inline footnote] definition.

Duplicated footnote reference[^second].

[^first]: Footnote **can have markup**

    and multiple paragraphs.

[^second]: Footnote text.


### [Definition lists](https://github.com/markdown-it/markdown-it-deflist)

Term 1

:   Definition 1
with lazy continuation.

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.

_Compact style:_

Term 1
  ~ Definition 1

Term 2
  ~ Definition 2a
  ~ Definition 2b


### [Abbreviations](https://github.com/markdown-it/markdown-it-abbr)

This is HTML abbreviation example.

It converts "HTML", but keep intact partial entries like "xxxHTMLyyy" and so on.

*[HTML]: Hyper Text Markup Language

### [Custom containers](https://github.com/markdown-it/markdown-it-container)

::: warning
*here be dragons*
:::

# Do Monads Matter?

### Functional programming for people who hate math.

by [Jason Lengstorf](https://code.lengstorf.com/)
[@jlengstorf](https://twitter.com/jlengstorf) | [[email protected]](/cdn-cgi/l/email-protection#630902100c0d230f060d0410170c11054d000c0e)

Slides: [git.io/vyzvq](https://git.io/vyzvq)

## Who I Am

* i
* am
* annie
* tran
* github.io/nntrn

This joke is so terrible. You should be ashamed of yourself.  

## Who I Am

* Building web shit since 2003
* *Huge* process & efficiency nerd
* Work-life balance advocate / consultant
* Senior developer at IBM
* Author of 3 books on development stuff
* World champion purveyor of bear hugs

<details>
<summary><mark>random javascript notes</mark></summary>
  

## What is *functional programming*?

### What does this mean?

```
(s → a) → ((a, s) → s) → Lens s a
Lens s a = Functor f => (a → f a) → s → f s
```

(If you *do* understand this, now would be a good time to fake an urgent phone call.) 

  This is the "signature" of the Lens function in Ramda. I have no idea what this means.  

### To accomplish this, our code follows a few rules:

1. Functions are better than loops
2. Always return the same result given the same arguments
3. Write functions that do one thing

## Let's *learn how*

### Rule \#1:

## *Functions *Are Better Than

# **Loops**

### Scenario: This Beverage List

## Is **Broken**

```js
const people = [
{
  name: 'Marisa',
  spirit_animal: 'koala',
  beverages: [
    'tea',
    'vodka', // <-- WTF is this?!
  ],
},
{
  name: 'Jason',
  spirit_animal: 'bear',
  beverages: [
    'coffee',
    'whiskey',
  ],
},
];

```

First: a quick bit of ~~jargon~~ vocabulary.

### **Imperative** Programming

Code that explicitly describes **how to do something**.

#### An **Imperative** Approach to Eating:

![When Harry Met Sally](RIL_assets/code.lengstorf.com/presentations/functional-programming/slides/images/functional-programming/imperative-sally.jpg)
 "I'd like the pie heated and I don't want the ice cream on top, I want it on the side, and I'd like strawberry instead of vanilla if you have it. If not, then no ice cream, just whipped cream — but only if it's real; if it's out of the can then nothing." 

### *Declarative* Programming

Code that describes **what the result should be**.

#### A *Declarative* Approach to Eating:

![Parks and Recreation](RIL_assets/code.lengstorf.com/presentations/functional-programming/slides/images/functional-programming/declarative-ron.jpg)
"Give me all the bacon and eggs you have."

  Tyler McGinnis has a couple great metaphors  

## Got it?

Let’s look at some code.

### An **Imperative** Solution

```
let fixed = [];
for (let person of people) {
if (person.beverages) {
  for (let beverage in person.beverages) {
    if (person.beverages[beverage] === 'vodka') {
      person.beverages[beverage] = 'whiskey (FTFY)';
    }
  }
}
fixed.push(person);
}
```

Try this live: <https://goo.gl/aobHwP>

## Beware the **Pyramid of Doom**!

 ![Pyramid of Doom by Contenebratio](RIL_assets/code.lengstorf.com/presentations/functional-programming/slides/images/functional-programming/pyramid-of-doom.jpg) Credit: [Contenebratio](http://rdbl.co/2m8qRfP)  

### A *Declarative* Solution

```
const fixBeverage = (str) => (
str.replace('vodka', 'whiskey (FTFY)')
);

const helpIfConfused = (person) =\> ({
 ...person,
 beverages: person.beverages.map(fixBeverage)
 });

`const fixed = people.map(helpIfConfused);`

```

Try this live: <https://goo.gl/HO7tps>

### The Result Is *Identical*

```
[
{
  "name": "Marisa",
  "spirit_animal": "koala",
  "beverages": [
    "tea",
    "whiskey (FTFY)"
  ]
},
{
  "name": "Jason",
  "spirit_animal": "bear",
  "beverages": [
    "coffee",
    "whiskey"
  ]
}
]

```

## Okay but...

## What the eff's a

# *map*?

### `Array.prototype.map()`

Applies a function to each element of an array.

### Which means that **this**...

```
const double = num => num * 2;
const numbers = [1, 2, 3];
const nextNumbers = [];
for (let x in numbers) {
nextNumbers[x] = double(numbers[x]);
}
```

Try this live: <https://goo.gl/30SfNQ>

### ...is the same as *this*.

```
const double = num => num * 2;
const numbers = [1, 2, 3];
const nextNumbers = numbers.map(double);
```

Try this live: <https://goo.gl/7mYn2x>

### Protip: get comfortable with *array methods*

* `Array.prototype.filter()`
* `Array.prototype.sort()`
* `Array.prototype.every()`
* ...and [many more](https://mzl.la/2mlIQPH).

### Rule \#2:

## The Same Input*Always*Returns the
Same Result

### "Wait. That's dumb. My code already does that."

## Are you **sure**?

### The Jargon:

# *Pure* vs. **Impure**

### Scenario: Tell People About Your *Favorite* Thing

### An **Impure** Solution

```js
let myFavoriteThing = 'whiskey';

function describeMyFavoriteThing() {

return `I prefer to drink quality ${myFavoriteThing}.`;

}
```



Try this live: <https://goo.gl/IQeD45>

### Wait! New feature request:

```js
function clarifyFavoriteThing() {
myFavoriteThing = 'aged ' + myFavoriteThing;
}
```

Try this live: <https://goo.gl/FEUtUZ>

### Then Legal Gets Involved:

```js
function undergoMajorLifeChanges() {
myFavoriteThing = 'scented bubble bath';
}
```

Try this live: <https://goo.gl/RcBsDc>

### Good Luck Debugging This:

```js
let myFavoriteThing = 'whiskey';

clarifyFavoriteThing();
 describeMyFavoriteThing();
 //=\>"I prefer to drink quality aged whiskey." (yay!)

// ...probably a bunch of additional code...
 undergoMajorLifeChanges();
 // ...probably more additional code...

```


Try this live: <https://goo.gl/AUVt8n>

 This is hard to debug and we *just wrote it*. Imagine coming back to this in six months, or inheriting this code from a team member and having no idea what each of these functions is supposed to be doing.  

### A *Pure* Approach

```js
function describeMyFavoriteThing(beverage) {
return `I prefer to drink quality ${beverage}.`;
}

function clarifyFavoriteThing(favoriteThing) {
 return `aged ${favoriteThing}`;
 }


function undergoMajorLifeChanges() {

return 'scented bubble bath';

}
```



Try this live: <https://goo.gl/zcxJVN>

### We can clearly follow what's happening:

```js
const myFavoriteThing = 'whiskey';
const clarified = clarifyFavoriteThing(myFavoriteThing);
const newFavorite = undergoMajorLifeChanges();

describeMyFavoriteThing(myFavoriteThing);
 //=\>"I prefer to drink quality whiskey."

describeMyFavoriteThing(clarified);
 //=\>"I prefer to drink quality aged whiskey."


describeMyFavoriteThing(newFavorite);

//=>"I prefer to drink quality scented bubble bath."
```



Try this live: <https://goo.gl/zcxJVN>

### Debugging is *easy*:

```
// start debugging here: ↓ ↓ ↓ ↓ ↓
describeMyFavoriteThing(newFavorite);
```

Try this live: <https://goo.gl/zcxJVN>

### This Is Called *Referential Transparency*

 This means the function call can always be replaced with its return value without breaking the program. 

### We can replace any pure function with its return value & get the *same result*:

```
const chz = 'I love ' + clarifyFavoriteThing('cheddar');
```

...is the same as...

```
const chz = 'I love aged cheddar.';

```

### Testing's Never Been *Easier*:

```
expect(clarifyFavoriteThing('cheddar'))
.toEqual('aged cheddar');

```


## Rule \#3:

### Each Function Does*One Thing*

#### Scenario: Filter by Genre &Sort by *Artist*

```js
const albums = [
{
  name: 'Middle Cyclone',
  artist: 'Neko Case',
  genre: 'indie',
},
{
  name: 'Highly Refined Pirates',
  artist: 'Minus The Bear',
  genre: 'rock',
},
{
  name: 'Rabbit Fur Coat',
  artist: 'Jenny Lewis',
  genre: 'indie',
},
{
  name: 'Black on Both Sides',
  artist: 'Mos Def',
  genre: 'hip-hop',
},
];

```

### An **All-In-One** Solution

```js
function getOnlyIndie(albums) {
let filtered = [];
for (let album of albums) {
  if (album.genre === 'indie') {
    filtered.push(album);
  }
}
filtered.sort((album1, album2) => {
  if (album1.artist === album2.artist) return 0;
  return album1.artist > album2.artist ? 1 : -1;
});
return filtered;
}
```

Try this live: <https://goo.gl/lPK1CD>

### *One Function* Per Step

```js
const byArtistAsc = (album1, album2) => {
if (album1.artist === album2.artist) {
  return 0;
}

return album1.artist \> album2.artist ? 1 : -1;
 };

const getOnlyIndie = (album) =\> {
 return album.genre === 'indie';
 };

`albums.filter(getOnlyIndie).sort(byArtistAsc);`

```

Try this live: <https://goo.gl/VVjFSZ>

## But Wait!

We can do even better.

### This is *so freakin' reusable*!

```js
const filterByGenre = R.curry((genre, album) => {
return album.genre === genre;
});


const onlyHipHop = filterByGenre('hip-hop');

const onlyIndie = filterByGenre('indie');

const onlyRock = filterByGenre('rock');
```



Try this live: <https://goo.gl/qPJhZW>

### What's That *Curry* Thing?

...besides delicious, that is.

### `R.curry()`

Allows functions to be called in stages.

  We’re using Ramda for these examples, but currying is not a Ramda-only feature: you can write your own currying function in any programming language, and many libraries (such as lodash) offer a currying function.  

### Which allows us to do this:

```js
function addNumbers(num1, num2) {
return num1 + num2;
}

const curriedAdd = R.curry(addNumbers);
 const add4 = curriedAdd(4);

add4(2); //=> 6

add4(7); //=> 11

```

Try this live: <https://goo.gl/jVjOW3>

# Let's *Recap*

### Functional programming
helps us write code that is:

* Easier to understand and debug
* Cheaper and easier to maintain
* More legible
* More reusable
* More testable
* Less error-prone

### To accomplish this, our code follows a few rules:

1. Functions are better than loops
2. Always return the same result given the same arguments
3. Write functions that do one thing

### You can *go deeper*...

 ...but just these three techniques will save you hours of headaches and make your code better and easier to deal with going forward. 

# Questions?

Jason Lengstorf
[@jlengstorf](https://twitter.com/jlengstorf) | [[email protected]](/cdn-cgi/l/email-protection#1973786a767759757c777e6a6d766b7f377a7674)

### Resources

1. [Favoring Curry](http://fr.umio.us/favoring-curry/)
2. [Introduction to Composition in JS](http://blog.ricardofilipe.com/post/javascript-composition-for-dummies)
3. [Ramda, a functional library for JS](http://ramdajs.com/)
4. [Array methods in JavaScript](https://mzl.la/2mlIQPH)
5. [Imperative vs Declarative Programming](https://tylermcginnis.com/imperative-vs-declarative-programming/)

Tweet: [@jlengstorf \#oraclecode](https://twitter.com/intent/tweet?text=Do%20Monads%20Matter%253F%20by%20%2540jlengstorf&hashtags=oraclecode&related=jlengstorf%252Coracledevs&url=https%253A%252F%252Fcode.lengstorf.com%252Fpresentation%252Ffunctional-programming%252Fslides%252F)

This is just a sample. You can play around with your own text right here.

</details>


Markdown
-------------

...is really just ordinary text, *plain and simple*. How is it good for you?

- You just **type naturally**, and the result looks good.
- You **don't have to worry** about clicking formatting buttons.
  - Or fiddling with indentation. (Two spaces is all you need.)

To see what else you can do with Markdown (including **tables**, **images**, **numbered lists**, and more) take a look at the [Cheatsheet][1]. And then try it out by typing in this box!

[1]: https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet

<style>

.scroll {height:100px; overflow:scroll;

}

</style>

