# Math Folder

The Math blocks are used for
[numbers](https://arcade.makecode.com/types/number), number operators,
and math functions.

-   For more information and examples on the Math blocks, go to
    <https://arcade.makecode.com/reference/math>

## Numeric values: 0, 1, 2, 6.7, 10.083…

Just numbers by themselves. Sometimes these are called *numeric
literals*.

## Integers: whole numbers

<img src="../images/media/image78.png"
style="width:3.11111in;height:2.30556in"
alt="A red rectangular object with white text Description automatically generated" />

## Floating point: numbers with a fractional part

Numbers can have their fractional part too. The decimal point is between
the digits of the number. But, *floating point* numbers have the decimal
point at any spot between digits, like: 3.14159 or 651.75.

<img src="../images/media/image79.png" style="width:3.59722in;height:2in"
alt="A screenshot of a computer Description automatically generated" />

## Arithmetic binary operation (+, -, \*, /)

The operations for basic arithmetic: add, subtract, multiply, and
divide.

<img src="../images/media/image80.png"
style="width:5.01389in;height:3.08333in"
alt="A screenshot of a red and purple math program Description automatically generated" />

## Remainder (%)

This is a extra operator for division. You can find out how much is left
over if one number doesn’t divide into the other number evenly.

We know that 4 / 2 = 2, so 2 divides into 4 evenly. But, 5 / 2 = 2 with
a remainder of 1. So, the remainder operation, 5 % 2 = 1, gives the
number that’s left over from a division operation.

<img src="../images/media/image81.png"
style="width:6.19444in;height:1.05556in"
alt="A purple and pink rectangle with white text Description automatically generated" />

## Exponent (\*\*)

The exponent operator will multiply the number on the left by itself for
the amount of times of the number on its right. That is, 4 \*\* 2 = 4 \*
4 and 2 \*\* 3 = 2 \* 2 \* 2. The area of a square that has sides with a
length of 5 is equal to one side multiplied by another. For a square,
all sides are equal, so:

<img src="../images/media/image82.png"
style="width:5.77778in;height:1.95833in"
alt="A screenshot of a computer Description automatically generated" />

But using the exponent operator, this is the same as:

<img src="../images/media/image83.png"
style="width:6.02778in;height:1.98611in"
alt="A red and purple rectangular object with white text Description automatically generated" />
The volume of a cube is three sides multiplied together. The two volumes
are the same:

<img src="../images/media/image84.png"
style="width:6.5in;height:2.13681in"
alt="A red and purple rectangular buttons with white text Description automatically generated" />

## Integer multiply and divide

Integer multiply and divide treats the two numbers it operates on as
integers. If there is a fractional part for a number, it is truncated
before it is used with the other number. The resulting value is always
an integer too.

## Imul – Integer Multiplication

Integer multiplication of two numbers 3.9 and 4.2 results in a value
of 12 since just the values of 3 and 4 are used from the numbers
multiplied.

<img src="../images/media/image85.png"
style="width:6.45833in;height:1.97222in"
alt="A screenshot of a computer Description automatically generated" />

##  idiv – Integer Division

Integer division of two numbers 7.8 and 2.6 results in a value
of 3 since just the values of 7 and 2 are used from the numbers
multiplied.

<img src="../images/media/image86.png"
style="width:6.08333in;height:1.81944in"
alt="A screenshot of a computer Description automatically generated" />

## Square root

The square root of a number is another number that when multiplied by
itself it becomes the original number. You know that 2 \* 2 equals 4 so
the square root of 4 is 2. It’s called a *square root* because the area
of a *square* is the length of two equal sides multiplied together.
The *root* is the length of a side.

<img src="../images/media/image87.png"
style="width:6.40278in;height:2.59722in"
alt="A screenshot of a computer program Description automatically generated" />

## Absolute value

When you want to know how much a number is without its *sign* (+/-). The
absolute value of -5 is 5 and the absolute value of 5 is also 5. The
absolute value is sometimes called the *magnitude*.

<img src="../images/media/image88.png"
style="width:5.01389in;height:1.38889in"
alt="A red and purple rectangle with white text Description automatically generated" />

-   For more information on absolute block, go to
    <https://arcade.makecode.com/reference/math/min>

##  Minimum and maximum of two values

You can get the smaller or the bigger of two numbers with
the [min](https://arcade.makecode.com/reference/math/min) and [max](https://arcade.makecode.com/reference/math/max) functions.

-   The minimum of 2 and 9: **Math.min(2, 9)** equals 2.

-   The maximum of 3 and 9: **Math.max(3, 9)** equals 9.

<img src="../images/media/image89.png"
style="width:6.25in;height:1.86111in"
alt="A screenshot of a computer Description automatically generated" />

## For more information on max block, go to <https://arcade.makecode.com/reference/math/max>

-   For more information on min block, go
    <https://arcade.makecode.com/reference/math/min>

## Round

If a number has a fractional part, you can make the number change to be
the closest, next integer value. This is called *rounding*. Rounding the
number 6.78 will make it be 7 and rounding 9.3 will give you 9. If a
number has a fractional part greater than or equal to 0.5, the number
will round up to the next whole integer value with the higher value.
Otherwise, it will round down to the next lowest integer value.

For negative numbers, they round toward the absolute value (the absolute
value of -8 is 8) of the number. So, -5.23 rounds to -5 and -2.68 rounds
to -3.

<img src="../images/media/image90.png"
style="width:5.20833in;height:1.18056in"
alt="A red and purple rectangular sign Description automatically generated" />

##  Ceiling

To make a number change to the next higher whole number (integer), get
the number’s *ceiling* value. The ceiling value for 1.234 is 2 since
that is the next higher whole number. For the negative number of -3.63,
its ceiling is -3 since that’s the next higher whole number.

<img src="../images/media/image91.png"
style="width:5.71637in;height:1.09511in"
alt="A red and purple rectangular sign Description automatically generated" />

## Floor

To make a number change to the next lower whole number (integer), get
the number’s *floor* value. The floor value for 8.76 is 8 since that is
the next lower whole number. For the negative number of 6.17, its floor
is -7 since that’s the next lower whole number.

<img src="../images/media/image92.png"
style="width:5.16976in;height:0.96298in"
alt="A red and purple button with white text Description automatically generated" />

## Truncate

The fractional part of a number is removed by *truncating* it. If a
number has the value 54.234 its truncated value is 54. Truncation works
the same way for a negative number. The truncated value
of -34.913 is -34.

## <img src="../images/media/image93.png"
style="width:6.27625in;height:1.14621in"
alt="A red and purple rectangular button with white text Description automatically generated" /> Random value

Make up any number from a minimum value to a some maximum value. If you
want a random number up to 100, say: **Math.randomRange(0, 100)**.

<img src="../images/media/image94.png"
style="width:6.49247in;height:1.01326in"
alt="A red and purple rectangle with white text Description automatically generated" />