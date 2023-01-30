# The Ghist
An extention of [[Double Integration]].

Part of a series on #Mathematics/Calculus 

# The Mathematics
[[Foubinie's Thoerem]] holds well, thankfully.

For the integral for $dzdydx$ we first gather the "shadow" of an object over the $xy$ plane (also known as $R$ for convention). This is usually grabbed as a [[Double Integration]]:$$R=\int_{P_0}^{P_1}\int_{g_(0)}^{g_1(x)}dxdy$$Then, we extend this to the third dimension.

# Examples
### Tetrahedron with vertices (0,0,0), (1,1,0), (0,1,0) and (0,1,1). Use $dydzdx$:
Start with the projection of the shape onto the plane $dzdx$, as they are the latter two variables in the integration order. This means that our "in" section will be a function of $y$, and the "out" section will be a constant of $y$.

Given our points, we can now create an equation of a [[Plane]] using the normal methods (cross product of two touching vectors to generate a normal vector):$$1(x-0)-1(y-0)+(z-0)=0 \rightarrow z-y+z=0$$Now simply solve for $y$:$$y=x+z$$This is our "in" value as mentioned previously. Our "out" constant is $y=1$. Therevore, we now have $$\int_{x+z}^1dydzdx$$Add in our other two integrals:$$\int_0^1\int_0^{1-x}\int_{x+z}^1dydzdx$$

### Same region over $dzdydx$
Now, our region $R$ lies along $yx$. Our strips along $R$ can most easily be taken from $x=y$ and $x=0$.

We'll go "in" at a constant of $z$, and out at a function of $z$. Use the plane found earlier to calculate this. $$\int_0^1\int_x^1\int_0^{y-x}dzdydx$$

### Average Value of a Function in Space
Simply find the value over the region($D$), then divide the triple integral of the function over the space by that. Frr the cube with side lengths two, the integral for the function $f(x,y,z)=xyz$ is easily$$\int_0^2\int_0^2\int_0^2xyzdxdydz$$Now divide by the space. This could be done with an integral, but with a cube the answer is simply $8$. The average value here is thus $1$.

### Region the integral $\int_{-1}^1\int_{x^2}^1\int_0^{1-y}dzdydx$
Rewrite in the order:
#### $dydzdx$:
