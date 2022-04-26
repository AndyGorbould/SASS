SASS



Being able to explain what a CSS-Preprocessor is
        a thing.... 

Generate some CSS from your CSS preprocessor (SASS)
        the $ worked & the @mixins work

Being able to minify your CSS output
        removes all the spacing & tabbing to make the whole CSS into one long line?? I've seen it but haven't implemented it yet

Knowledge of the following SASS features:

Variables
    vars in SASS start with an $, they are (normally) declared at the beginning of the file & refered to in the normal css method:
            h6 {
            color: $primary;
        }


Mixins (Functions)
    @mixin NAME { standard css syntax, color:, margin:, etc}
    mixin= combo
    declare with @include NAME eg
        body {
            @include lots-of-styling;
        }


Nesting
        makes the SCSS easier to read & navigate, & reduces typing the same thing twice & reduces typing the same thing twice ;)

Partials & Import
    with _filename you can have a small, re-usable piece of code that can be re-used if you're doing the same task multiple times - very efficient!

Extend/Inheritance


Operators (Math)
        eg. padding: $padding-general * 2;   this doubles(*2) the $padding-general var






Must-have features
Your mission is to rewrite the example.css to a scss file with the following changes:

Part 1
Make one mixin for the 3 lines of the box-shadow styling.

Make the general padding the same everywhere with one variable. (red=16px, blue=8px), the footer h6 should have double the padding of the other elements. Use "operations" to do this. Do NOT hardcode the padding inside your scss.

Nest the styling rules of grouped elements, like the sections in the Article.

Make use of extend to re-use the same CSS for the "success", "error" and "warning" messages.

Part 2 (optional)
Add an option to your compilation to minify your stylesheet! Mine was below 1.6k, can you do better? Do you still remember the option to ls to make the filesize Human readable?