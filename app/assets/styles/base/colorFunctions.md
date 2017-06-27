body {
  background: color(red a(90%))
}
you will get:

body {
  background: rgba(255, 0, 0, 0.9)
}

whatever {
  color: color(red a(10%));

  background-color: color(red lightness(50%)); /* == color(red l(50%)); */

  border-color: color(hsla(125, 50%, 50%, .4) saturation(+ 10%) w(- 20%));
}

[red( | green( | blue( | alpha( | a(] ['+' | '-']? [<number> | <percentage>] )
[red( | green( | blue( | alpha( | a(] '*' <percentage> )
[hue( | h(] ['+' | '-' | '*']? <angle> )
[saturation( | s(] ['+' | '-' | '*']? <percentage> )
[lightness( | l(] ['+' | '-' | '*']? <percentage> )
[whiteness( | w(] ['+' | '-' | '*']? <percentage> )
[blackness( | b(] ['+' | '-' | '*']? <percentage> )
tint( <percentage> )
shade( <percentage> )
blend( <color> <percentage> [rgb | hsl | hwb]? )
contrast( <percentage>? )