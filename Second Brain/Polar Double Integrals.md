# The Ghist
Using [[Double Integration]] using polar functions.

Part of a series on #Mathematics/Calculus 

# The Mathematics
The challenge in this secion is moving from $dxdy$ to $d\theta dR$. There isn't an easy solution to this unfortunatly. It is essentially an analouge$$dA=dxdy\rightarrow dA= drd\theta$$The area of a segment is $A=\dfrac{1}{2}\theta r^2$, so we may state $A_k = r_k \Delta r \Delta \theta$, or $$dA=rdrd\theta$$This is the founding principle of polar work in this system. Our general form is $$A=\int_\alpha^\beta\int_{r_1(\theta)}^{r_2(\theta)}rdrd\theta$$This is where [[Double Integration]] really shines, as it vastly improves over the single [[Integral]] form of previous explorations

## Limits of Integration
The inner limit will be the variable $r$, and the outer limit $\theta$
### For region R:
```desmos-graph
bottom = 1.2; top = 3
left = 0; right = 2
---
y(x) = \sqrt 2
x^2+y^2=4
```
For the inner rules, set up the solution as a pair of equations and solve

$$rsin\theta=\sqrt{2} \rightarrow r=\sqrt2 csc\theta$$

### For region inside$r= 1 + cos\theta$ and outside $r=1$
```desmos-graph
left = -2; right = 4;
top = 2; bottom = -2;
---
r = 1 + \cos(\theta)
r = 1
```
For our inner integral, we simplly use $r=1$ and $r = 1+\cos \theta$. For the outer section use $\dfrac{\pi}{2}$ and $-\dfrac{\pi}{2}$:$$\int_{-\dfrac{\pi}{2}}^{\dfrac{\pi}{2}}\int_1^{1+\cos\theta}f(r,\theta)rdrd\theta$$First we sweep over $r$, then $\theta$.


## Area of Region

### $r^2=4\cos(2\theta)$
```desmos-graph
r=\sqrt{4\cos{2\theta}}
```
Remember out limits, $r$ and $\theta$. Here only 0.25 of the area is in the first coordinate, so we may multiply by four. Enter at $0$ and exit at $\sqrt{4\cos(2\theta)}$. Sweep over the area from $0$ to $\dfrac{\pi}{4}$. Therefor our integral is $$A_{\dfrac{1}{4}}=\int_0^{\dfrac{\pi}{4}}\int_0^{\sqrt{4\cos(2\theta)}}rdrd\theta$$Integration of this problem is fairly simple, given the $0$'s in the lower position. 

### $\int\int e^{x^2+y^2}dydx$

$R$ here is a semicircular region bounded by the x-axis and the curve $y=\sqrt{1-x^2}$. Solve using $x^2+y^2 = r^2$ $$\int\int e^{x^2+y^2}dydx=\int_0^{\pi}\int_0^1 e^{r^2}rdrd\theta$$Solve normally

### $\int\int(x^2+y^2)dydx$
```desmos-graph
x^2+y^2=1
```
Region is first quadrant of a circle, so the integral is trivial $$\int_0^{\dfrac{\pi}{4}}\int_0^1 r^2rdrd\theta$$Solve normally.

### Volume of region bounded by $z=9-x^2-y^2$ and the unit circle placed on the $xy$ plane
Function solved for $r\theta$:$$f(r,\theta)=9-r^2$$
Circular Integration: $$\int_0^{2\pi}\int_0^1(9-r^2)rdrd\theta$$Integral solution is trivial.