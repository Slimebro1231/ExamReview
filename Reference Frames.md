So, reference frames. Fun. Usually, when we set a reference frame, we need a "subject." Then, we lock the camera to the subject, which means the subject is stationary "relative" to the camera.

Here is an example. You have a person walking on a moving bus. If we had our "camera", or "frame of reference" set to the ground, in our view, the ground is not moving. The person is moving at a different speed to us than the bus, with the bus moving as well. 

However, If we set our "reference" to the bus, the bus doesn't seem like it is moving to us, right? since the camera is stuck to the bus. On the contrary, if we look outside the window, the ground is "moving", so is the person inside.

If we again placed our camera on the ground, and instead measured the velocities of the person relative to the ground, and the velocity of the bus relative to the ground, we will realize that the person is actually moving **super** fast, to be exact, nearly the speed of the bus.

To calculate exactly how fast the person is actually walking, we can do vector subtraction, as shown in [[vector components]].


Another thing that is really important about reference frames, which is rotation. 

We had only previously covered relative **Motion**, but what if both objects are stationary? If we have a block setting on a ramp, we may want to set our "reference frame" to something that is at an angle. 

![[Slope.png]]

Here is an explanation of this part. So we have the $F_g$ , which right now looks like this:
$$
\begin{bmatrix} 
0\\ 
m*g
\end{bmatrix}
$$
As the red line is perpendicular to the ground, meaning there is no x component to it. 

However, if we put our reference frame on the block, things change. 

We use what is known as a rotation matrix, which for the sake of a matrix like 0,1; It can just be simplified to this:
$$\begin{matrix} 
x'\\
y'
\end{matrix}
=
\begin{bmatrix} 
cos\theta & -sin\theta\\ 
sin\theta & cos\theta
\end{bmatrix}
\begin{bmatrix} 
x\\
y
\end{bmatrix}
$$
You will soon learn this in calculus, as this is vector multiplication, but for simplicity's sake, here is the result:

$$\begin{bmatrix} 
x'\\
y'
\end{bmatrix}
=
\begin{bmatrix} 
x cos\theta - y sin\theta\\ 
x sin\theta + y cos\theta
\end{bmatrix}
$$
So since x is 0 in this case, as there is no x component, it simply becomes:
$$\begin{bmatrix} 
x'\\
y'
\end{bmatrix}
=
\begin{bmatrix} 
-sin\theta\\ 
cos\theta
\end{bmatrix}
$$
> Important!
> These rotations are counterclockwise, and $F_g$ is a negative value

This means that after you use this, the $y$ value is a negative, which is **Correct** 
The demonstration in the graph gives scalar values, and is a simplified version of this. 

Regardless, if you don't care about the sign, and only the scalar value ( you should ), here is a summary for an object on a slope of angle $\theta$ :
$$ sin(\theta) \rightarrow x; \quad cos(\theta) \rightarrow y$$
