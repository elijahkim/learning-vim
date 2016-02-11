#The meat and potatoes

#Writing stuff!

I'm sure you want to learn how to insert text. Fine. That's understandable. Last
section I taught you how to get into it using `i`. But that's just the
beginning.

Word of warning
---------------

Unless you're writing, you really shouldn't be in insert mode. Staying in insert
mode and moving around with the cursor keys, deleting 1 letter at a time because
you messed up, etc etc is pretty much an anti pattern. Try your hardest to only
go into insert mode to type.

##So insert mode?

```
`i` - Start insert mode under the cursor
`a` - Start insert mode to the right of the cursor
`o` - Start insert mode on the next line
`O` - Start insert mode on the previous line
```

You should practice and get used to these commands.

#Life outside of insert mode

As a developer, you're going to be moving things around or editing code in
various places. Keeping this in mind, Vim has very quick ways of moving the
cursor around a codebase and editing.

##Motions

These are ways to navigate the cursor

```
`gg` - Brings the cursor to the top of the page
`G` - Brings the cursor to the bottom of the page
`w` - Beginning of next word
`e` - End of next Word
`b` - Back one word
`0` - Beginning of line
`$` - End of line
`}` - Next blank line
`{` - Previous blank line
```

##Operators

You use these to do stuff

```
`y` - Yank
`d` - Delete
`r` - Replace
`p` - Paste
`x` - Delete under cursor
```

##The Magic of composition

Vim is pretty cool because you can compose actions and motions together. For
example, getting to the 20th line of a file is `20gg`. Wait what?

So you can compose things like `<operator><motion>` and this lets you do very
powerful things.

```
Some Example lorem
that spans multiple
lines. Like this.
So that we can practice.
A line with a lot of words so we can practice a lot more!
```

Let's assume we want to delete the word `Example` from line 41. You can do it
like this:

1. `41gg` to get to the 41st line
2. `w` to get to the next word
3. `dw` to delete word

Assume you want to delete 3 words. How would that be accomplished? One solution
would be `d3w`. Pretty awesome!
