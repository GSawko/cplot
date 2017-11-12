## cplot

Linux and Windows port of the [Mac OS X](http://www.zoon.cc/cplot/) function plotter.

Its main function is to help understanding how some function (like the complex
exponential or the solution to some differential equation, say) actually works.

For that, it supports various projection modes and function types, natural expression
syntax (sin xy instead of Sin[x*y] f.i.), blending between functions (identity and your
target function for example), and realtime parameter variation (where parameters
are things like a mass or spring constant, order of a pole, etc).

Some screenshots are at the link above, but the interface is completely different
(and on Linux quite rubbish, tbh).

### Linux build needs:

- scons and g++
- libz, libpthread, libreadline
- libX11, libXinput2
- GL, GLU, GLEW
- pangocairo
- boost headers

After building (just *scons* or *scons --release*),
try ./cplot test.cplot, press 1 + left/right arrows to change n,
type *help* for command list, *g csc z^2* to change the function, *q* to quit, ...
It can actually do quite a bit more, but the UI does not exist yet.

### On Windows:

Open CPlot.sln in Visual Studio 2017, and it should just build.
