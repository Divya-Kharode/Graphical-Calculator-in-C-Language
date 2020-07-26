# Graphical Calculator

A GTK 3 based Scientific Calculator 

We need to install the GTK 3

See the install file

## Demo

[![SC2 Video](https://i.ytimg.com/vi/KlEVS_aTkUw/hqdefault.jpg?sqp=-oaymwEZCPYBEIoBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLA-VpjRghVSSdsDk6t-NEDA8cHjtg)](https://youtu.be/KlEVS_aTkUw)

## For installation refer this site
https://askubuntu.com/questions/101306/how-do-i-install-gtk-3-0

## For Executing The Program
### Steps
    1. Download git repository
    2. Change the current working directory to your local project.
    3. Run the Command
        $ gcc `pkg-config --cflags gtk+-3.0` -Wall -o example calci.c `pkg-config --libs gtk+-3.0` -lm
        $ ./example
    


# Operations


This part of calculator is developed actively. This section gives an overview 
of the functions currently implemented and points out some restrictions.

Formula entry mode accepts integers as a input of +, -, *, /, %, ^ operations.
All algebraic operations and functions of the algebraic mode are supported. The 
following table lists all available operations:

Operation			identifier	
+, -, *, /			+, -, *, /
mod (%)				%
power x^y			^
ceil				┌ 
absolute			||
floor				└
*10^				*10^x

Let's speak of factorial. Most functions' argument 
has to be enclosed by brackets. Therefore sin 3 is not allowed and has to be 
written as sin(3).
Trignometric and logarithmic functions can be use for floating point value

Function			Function identifier	Example
Trigonometric functions: 
Sine, Cosine, Tangent		sin, cos, tan		sin(0.5)
their hyperbolic variants	sinh, cosh, tanh	sinh(0.5)
natural logarithm (base e)	ln			ln(3)
logarithm (base 10)		log			log(3)
square root			√ 			√ 3
factorial			!			3! brackets are 
							optional

# Some random notes

  * No floating values will respond for +, -, *, /, %, ^, It is only implemented for integer values.
  * Unlimited Precision is not handel yet still it can be done from -9223372036854775808 to 9223372036854775807 (8 Bytes)
    Number

