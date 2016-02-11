#Intro

##Vim - super customizable modal text editor

##First you may need convincing

Vim is a text editor that needs learning. It's painful to use from the beginning
and you're definitely going to be less productive for the first few weeks or
even a month. In other words, there is an extremely high barrier to entry.
However, once that threshold is crossed, the speed at which you can translate
your thoughts to text is second to none. As a developer, this ability is
crucial. The faster you can write, the fast you can edit, the faster you can
code.

Compare that with an IDE like sublime text. There is nearly no barrier to entry
and your productivity will stay stale nearly the whole time you use it. You
constantly, have to rely on a mouse which slows down development. "Hah! That's
merely seconds you say" but think about how many times you go back and forth
from the mouse to the keyboard. Once you learn vim, you'll see how barbaric this
is. You'll wonder how you survived for so long on such a terrible piece of
technology and you'll wish every app you used had vim bindings.

Lastly, why use a piece of technology to develop on that is so limited. I
understand that you can include plug-ins to your limited IDE but with vim you're
constantly improving and constantly getting faster. You can _never_ finish
learning vim. As a developer, this is extremely alluring to me. But maybe that's
just me.

So let's get started.

##Modal you say?

* Vim is modal in the sense that there are modes that you enter and exit in
  order to achieve your goal.

When you open a file through vim, you are dropped into the editor in `Normal
Mode`. You're going to be in this mode most of the time you're in vim. Here you
can move around, delete, paste, and a number of other things.

Movement
--------

h - left
j - down
k - up
l - right

* Don't use the arrow keys. The whole point of vim is to stay on the home row
  for as often as possible. Using the arrow keys is an anti-pattern.

As an editor, you expect to be able to write. You do this by going into `Insert
mode` or pressing `i`. You do your writing and when you're done you exit by
using `esc`.

```
practice here:
Hello world
```

Then there's also `Visual Mode`. You get into this a number of ways one of which
is `v`. Visual mode is pretty much like highlighting with the mouse and lets you
run commands on them afterwards.

The last one you'll be using a lot is the `Command Mode`. You get into this mode
by pressing `:`. The most obvious command you want to learn is to save `:w` and
to quit `:q`, or both `:wq`.

Not too hard so far!

Practice moving around, getting into and out of insert mode, saving, and
quitting.
