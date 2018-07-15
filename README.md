# SublimeProcapy
Programmer's Calculator in Python for Sublime Text. This is an inline calculator to use inside any document view in Sublime Text. Use inside existing views (e.g. source files) for quick inline calculations or dedicate a blank/unsaved view to use as an embedded standalone calculator.

## Usage
Simply select an expression (or multiple expressions using multiple selections) and execute the calculator by pressing the keyboard shortcut and the selection(s) will be replaced by the result of the calculation. Alternatively, if there are no selections, the line of the cursor will be parsed and the result inserted on the line after it (also works with multiple cursors). This is useful when using it as a normal calculator to incrementally perform a sequence of calculations using the result of the previous calculation as input for the following calculation leaving each step in the series of calculations visible.

Procapy supports any valid Python, and will reduce the result of any expression to a number (or an error string if something did not parse correctly).

The default keyboard shortcuts are:

 * ALT-ENTER: Calculate decimal
 * CRTL-ALT-ENTER: Calculate hexadecimal
 * SHIFT-ALT-ENTER: Calculate binary
 * SHIFT-CTRL-ALT-ENTER: Calculate octal

## Built-in functions
In addition to the Python standard functions, math and cmath modules, Procapy adds the following functions that are useful in programming:

 * u(w,x): truncate x to an unsigned integer of width w.
 * u8(x), u16(x), u32(x), u64(x): truncate x to an unsigned integer of the indicated width.
 * i(w,x): truncate x to a signed integer of width w.
 * i8(x), i16(x), i32(x), i64(x): truncate x to a signed integer of the indicated width.

These are similar to the built-in function int(x) which will truncate to an integer of unlimited width.

## Examples
