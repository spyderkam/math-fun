# Mathematical Model for a Rigid Sphere Falling from a Plane

## Defining the System

A mathematical model requires clear definition of variables:

-   A rigid sphere with mass $m$ and diameter $d$
-   A plane flying at velocity $\vec{v}_{\mathrm{p}}$ with acceleration $\vec{a}_{\mathrm{p}}$ at altitude $h$
-   Earth's gravitational acceleration $\vec{g} = -g\hat{z}$ where $g \approx 9.81$ m/s²

## Coordinate System

Using a Cartesian coordinate system where:

-   Origin is at the point directly below the plane on the ground
-   $x$-axis points in the direction of the plane's initial velocity
-   $z$-axis points upward (opposite to gravity)
-   $y$-axis completes the right-handed system

## Initial Conditions

At the moment of release ($t = 0$):

-   Position of the sphere: $\vec{r}(0) = (x_0, y_0, h)$
-   Velocity of the sphere: $\vec{v}(0) = \vec{v}_{\mathrm{p}}(0)$

## Forces Acting on the Sphere

1.  **Gravitational Force**:
    
    $$\vec{F}_{\mathrm{g}} = m\vec{g} = -mg\hat{z}$$
    
2.  **Drag Force** (assuming a quadratic drag model):
    
    $$\vec{F}_{\mathrm{d}} = -\frac{1}{2}C_{\mathrm{d}}\rho A |\vec{v}_{\mathrm{rel}}|\vec{v}_{\mathrm{rel}}$$
    
    Where:
    
    -   $C_{\mathrm{d}}$ is the drag coefficient (approximately 0.47 for a sphere in turbulent flow)
    -   $\rho$ is the air density (which varies with altitude)
    -   $A = \pi(d/2)^2$ is the cross-sectional area of the sphere
    -   $\vec{v}_{\mathrm{rel}}$ is the velocity of the sphere relative to the air

## Equations of Motion

Using Newton's Second Law:

$$m\vec{a} = \sum \vec{F} = \vec{F}_{\mathrm{g}} + \vec{F}_{\mathrm{d}}$$

This gives us:

$$m\frac{d^2\vec{r}}{dt^2} = -mg\hat{z} - \frac{1}{2}C_{\mathrm{d}}\rho\pi\frac{d^2}{4}|\vec{v}_{\mathrm{rel}}|\vec{v}_{\mathrm{rel}}$$

## Component Form

Breaking this into component equations:

$$ 
\begin{align*}
&m\ddot{x} = -\frac{1}{2}C_{\mathrm{d}}\rho\pi\frac{d^2}{4}|\vec{v}_{\mathrm{rel}}|v_{\mathrm{rel},x} \\
&m\ddot{y} = -\frac{1}{2}C_{\mathrm{d}}\rho\pi\frac{d^2}{4}|\vec{v}_{\mathrm{rel}}|v_{\mathrm{rel},y} \\
&m\ddot{z} = -mg -\frac{1}{2}C_{\mathrm{d}}\rho\pi\frac{d^2}{4}|\vec{v}_{\mathrm{rel}}|v_{\mathrm{rel},z}
\end{align*}
$$
## Additional Considerations

1.  **Air Density Variation** with altitude:
    
    $$\rho(z) = \rho_0 e^{-z/H}$$
    
    Where $\rho_0$ is sea-level density and $H$ is the scale height (~8.5 km).
    
2.  **Wind Effects**: You might need to consider ambient wind velocity $\vec{v}_{\mathrm{wind}}$ when calculating relative velocity:
    
    $$\vec{v}_{\mathrm{rel}} = \vec{v} - \vec{v}_{\mathrm{wind}}$$
    
3.  **Reynolds Number** effects on the drag coefficient:
    
    $$\mathrm{Re} = \frac{\rho|\vec{v}_{\mathrm{rel}}|d}{\mu}$$
    
    Where $\mu$ is the dynamic viscosity of air.
    
