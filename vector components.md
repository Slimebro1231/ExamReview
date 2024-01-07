Uh, not too hard, but extremely fundamental. 
I like to represent my components like this: $$\begin{bmatrix} x\\ y\end{bmatrix}$$Makes me seem pretentious? sure, but it will help very shortly.

So first things first, a vector, in most questions are not recorded in this {x, y} form, rather it is recorded as {length, direction}. And there are names for these two forms. 

> They are : 
> **Cartesian** {$x,y$}; also recognized as (Rect) on many calculators
> **Polar** {$r,\theta$}; also recognized as (Pol) on many calculators

Although it is important to remember how to do this by hand, doing it on a calculator is just honestly so much faster, and most teachers don't care. 

Before I get into how to convert between the two, here is a demonstration of what they are:

![[polCart 1.png]]
Essentially, Cartesian coordinates is just the x, y that we are familiar with, while polar includes the length of the vector, and the angle, which is usually what questions ask for.

Here is how to do it by hand ( quite simple)
So if we were to convert (1, 1) into polar, we would need the length of the vector and the angle.
This means: 
$$\begin{matrix} 
r\\
\theta 
\end{matrix}
\begin{bmatrix} 
\sqrt{x^2+y^2}\\ 
\arctan(y/x)
\end{bmatrix}$$

Right? Because the length is essentially the hypotenuse, which can be found using pythagorean's theorem, and the angle can be found using $arctan$, or some people call it $tan^{-1}$

Now converting from polar to Cartesian is the actual important part, because Cartesian coordinates can be "manipulated", as we will see in a bit. 
Conversion wise:
$$
\begin{matrix} 
x\\
y
\end{matrix}
\begin{bmatrix} 
r\space cos(\theta)\\
r\space sin(\theta)
\end{bmatrix}
$$
And this makes sense, because the $x$ component is just the Adjacent of the triangle, and $y$ is just the Opposite. 

After we convert to Cartesian, or Planar coordinates, we can do projectile motion! and practically everything. 

The whole point of this is to consider vectors components separately. So for example, we have a helicopter in the air, with a horizontal wind. The wind actually isn't affecting the rising part of the helicopter, so if we were to be concerned with displacement only:
$$
New \space Position:
\begin{bmatrix} 
x_0 + wind\\
y + lift
\end{bmatrix}
$$
The wind only affects the x component, which means we can just treat the x part of it as a 1D kinematics question, which can simply be done with the big 5. 

Now, This means that we can add many vectors together in the same way as well! 
So lets say we want to add a bunch of **forces**:
$$\vec{F_{net}}=\vec{F_1}+\vec{F_2}+\vec{F_n} \cdots$$
This can also be done as:
$$
\vec{F_{net}}=
\begin{bmatrix} 
F_1x\\
F_1y
\end{bmatrix}
+
\begin{bmatrix} 
F_2x\\
F_2y
\end{bmatrix}
+
\begin{bmatrix} 
F_3x\\
F_3y
\end{bmatrix}
\cdots
$$
Which can also be done as:
$$
\vec{F_{net}}=
\begin{bmatrix} 
F_1x + F_2x + F_3x\cdots \\
F_1y + F2y+F3y\cdots
\end{bmatrix}
$$
This makes things a LOT simpler when considering forces, as everything can just be added individually, and some forces are only apparent in one of the directions. 

After you have taken a look at relative motion, this will make sense:
So when considering [[Reference Frames]], we need this "subject" right. And the "subject" should be stationary, relative to our view. 

This means, to get the idk, velocity of $A$ relative to $B$, we can just subtract the velocity of B from A. 
Of course, velocity is a vector, so we use the same way:
$$
\vec{V_{AB}}=
\begin{bmatrix} 
V_Ax-V_Bx\\
V_Ay-V_By
\end{bmatrix}
$$
Oh, by the way, $\vec{V_{AB}}$ just means the velocity of A relative to B

Now, about setting different [[Reference Frames]], such as rotating, we will discuss there.
