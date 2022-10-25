Within an [[Integral]]:$$
\int f(g(x))g'(x)dx=f(u)du
$$and $$du=g'(x)dx$$Part of a series on #Calculus 

# Double Integrals
$$\int\int f(x,y)dxdy=\int\int f(g(u,v), h(u,v))j(u,v)dudv$$To substitute a [[Double Integration]] problem, the terms of the integrated function $f(x,y)$ must be written as $x(u,v)$ and $y(u,v)$. This process is called a transformation. Additionally, $u$ and $v$ must be represented as functions of $x$ and $y$. 

Then, the bounds of the integral must be adjusted to fit the new $uv$ space mapping, a process usually acheived by substitution. 

Finally, the function $f(x(u,v), y(u,v))$ must be multiplied by the [[Jacobian]] $j$, which is the determinant of the matrix 
$$\begin{matrix} \dfrac{\delta x}{\delta u} & \dfrac{\delta x}{\delta v} \\ \dfrac{\delta y}{\delta u}  & \dfrac{\delta y}{\delta v} \end{matrix}$$Afterwards, [[Integration]] may be performed normally.

## Examples