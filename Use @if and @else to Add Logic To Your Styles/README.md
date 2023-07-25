The @if directive in Sass is useful to test for a specific case - it works just like the if statement in JavaScript.

@mixin make-bold($bool) {
  @if $bool == true {
    font-weight: bold;
  }
}
And just like in JavaScript, the @else if and @else directives test for more conditions:

@mixin text-effect($val) {
  @if $val == danger {
    color: red;
  }
  @else if $val == alert {
    color: yellow;
  }
  @else if $val == success {
    color: green;
  }
  @else {
    color: black;
  }
}
Create a mixin called border-stroke that takes a parameter $val. The mixin should check for the following conditions using @if, @else if, and @else directives:

light - 1px solid black
medium - 3px solid black
heavy - 6px solid black
If the $val parameter value is not light, medium, or heavy, then the border property should be set to none.

Tests
Your code should declare a mixin named border-stroke which has a parameter named $val.
Your mixin should have an @if statement to check if $val is light, and to set the border to 1px solid black.
Your mixin should have an @else if statement to check if $val is medium, and to set the border to 3px solid black.
Your mixin should have an @else if statement to check if $val is heavy, and to set the border to 6px solid black.
Your mixin should have an @else statement to set the border to none.