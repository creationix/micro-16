# Primitive Value Types

- Integers (signed integer usually 64 or 32 bit depending on platform)
- Symbols (interned short strings)
- Buffers (raw mutable memory)
- Pairs (a value that holds two values)

# Composite Value Types

- Rationals (integer pairs as rationals)
- Lists (ordered linked list of values)
- Maps (any to any mapping)
- Objects (ports, internal state and handlers)

# Reference Types

- Pair values
- List values
- Map keys and values
- Function parameters
- Local variables

# Learning Sapphire

Sapphire is a scripting new scripting language aimed at being pleasant and simple.

Programs are organized into units of encapsulation known as objects.  If you
already know another programming language think of these as smalltalk objects
that receive messages, not java objects that have methods.

```sapphire
...this is a line comment

. this is an object definition
def Ball:
  . Define a couple internal variables that initialize to zero by default.
  x = 0 . x position on screen
  y = 0 . y position on screen
  angle = 0 . initial angle (0 is right, going counter-clockwise)
  velocity = 0 . initial velocity in pixels per tick

  tick: -- this will be hooked up to the main game event loop tick event.
    x += cos(angle) * velocity
    y += sin(angle) * velocity
    velocity *= 9/10

  kick:


ball = <Ball x=64 y=64>
```
