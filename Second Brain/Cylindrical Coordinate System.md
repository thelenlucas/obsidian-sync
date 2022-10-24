# Ghist
A [[Coordinate System]] that uses [[Polar Coordinate System]] terms and a z-axis to describe 3-D space. It is an extention of [[Polar Coordinate System]]s

Part of a series on #Calculus 

# Volume
The general volume formula is:$$\int\int\int dzrdrd\theta$$
# Examples
## Create the limiits of [[Integration]] over $D$ bounded by $z=0$, $x^2+(y-1)^2=1$, and $z=x^2+y^2$.

Remember the [[Polar Equivilence Equations]]s. The form of volume of a cylindrical coordinate space is$$\int\int\int dzrdrd\theta$$The plane $dz$ comes first. It enters at zero and exits at $z=x^2+y^2$.$$\int_0^{r^2}dz$$Next, find $r$ in terms of $\theta$. The $r$ bounds of this equatioon is a one-leaf [[Rose]], namely $r=2\sin\theta$. This integral level is thus $$\int_0^{2\sin\theta}dr$$Now, we simply have to find $\theta$ in terms of a constant. Because this [[Rose]] passes over the entire range of the one leaf, we can use [[Pi]] as our limit to gain. $$\int_0^{\pi}\int_0^{\sin\theta}\int_0^{r^2}dzrdrd\theta$$(Don't forget the $r$!)