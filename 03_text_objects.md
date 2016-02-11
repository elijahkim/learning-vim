#Text objects and more!

##Text Objects
Vim has a pretty cool construct called the `text object`. Text objects are kind
of what they sound like: an object of text. It can be a sentence, a word, or
even a paragraph. They're used in place of motions and can lead to many powerful
compositions.

One text object is `iw` or `Inner Word`

You can do a lot of things inner word. You can delete a word that the cursor is
in by doing `diw` or `Delete Inner Word` or you can yank the word `yiw` or `Yank
Inner Word`. Something I do a lot is `ciw` or `Change Inner Word`.

I'll just list some common text objects that I use:

```
iw - I mean cmon
aw - Around Word
i[ or ] - Inner [ or ] (I will no longer write both i and a)
a[ or ] - Around [ or ] (Anything with an inner has an around)
i( - Inner (
i" - Inner "
i' - Inner '
it - Inner Tag
```

I recently learned that `_` is the text object for current line so you can do
things like `d_` to delete the current line, `y_` to yank the current line etc.
However since operating on the same line is so commonly done, repeating an
operator does the same. So `dd` is the same as `d_` and `yy` is the same as `y_`

##The .

Whenever you do an action through composition you can use the `.` to do it
again. Let me explain through an example. Let's assume you have some ruby code
that looks like this:

```ruby
def speak(word)
  puts "word"
end

speak "hello"
speak "world"
```
and you want to change the method name from speak to say. You can find and
replace OR you can do it using `.`. Put the cursor over the word speak and type
`ciw`. This will delete the word and put you in insert mode. Type `say` and
escape out of insert mode. All of this was 1 action. Now whenever you press `.`
it will change that word to `say`. I think that's pretty cool.

##Closing words on composition

Composition is great because it allows you to do a lot of things without
memorizing tons of commands. For every operator you learn, you can apply it to
every motion or text object and vice versa. It's actually amazing.
