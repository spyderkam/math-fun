# Modeling the Radius of a Post-Impact Debris Cloud

To model the relationship between the radius of the cloud sphere ($R_{\mathrm{c}}$) and the original solid sphere ($R_{\mathrm{s}}$), We will analyze this problem using principles of mass conservation and packing density.

## Initial Conditions and Assumptions

-   We have a uniform solid sphere with radius $R_{\mathrm{s}}$
-   An interceptor traveling at the speed of light passes through this sphere
-   The sphere fragments into $N$ equivalent pieces of post-intercept debris (PID)
-   Each PID has volume much smaller than the original sphere
-   The PID form a cloud resembling a sphere with radius $R_{\mathrm{c}}$
-   The event occurs in a vacuum
-   Total mass is conserved (the sum of PID masses equals the original sphere mass)

## Mass Conservation Analysis

Since mass is conserved and the original sphere was uniform, the total volume of all PID pieces must equal the volume of the original sphere. However, the PID pieces are now distributed throughout a larger space with voids between them.

The volume of the original solid sphere is:

$$ V_{\mathrm{s}} = \frac{4}{3}\pi R_{\mathrm{s}}^3 $$

The volume of the spherical cloud is:

$$ V_{\mathrm{c}} = \frac{4}{3}\pi R_{\mathrm{c}}^3 $$

## Packing Density Model

The key insight is that while the actual material volume remains constant, the PID pieces no longer pack efficiently, creating empty space between fragments.

Let's define $\phi_{\mathrm{c}}$ as the packing fraction or packing density of the debris cloud, representing the fraction of the cloud volume that is actually occupied by material (with the rest being void space).

For the original solid sphere, the packing fraction $\phi_{\mathrm{s}} \approx 1$ since it was uniform and fully packed.

By conservation of mass: $\phi_{\mathrm{s}} V_{\mathrm{s}} = \phi_{\mathrm{c}} V_{\mathrm{c}}$.

Since $\phi_{\mathrm{s}} \approx 1$: $V_{\mathrm{s}} = \phi_{\mathrm{c}} V_{\mathrm{c}}$.

Substituting the formulas for spherical volumes: $\frac{4}{3}\pi R_{\mathrm{s}}^3 = \phi_{\mathrm{c}} \cdot \frac{4}{3}\pi R_{\mathrm{c}}^3$

Solving for the ratio of radii:

$$ \dfrac{R_{\mathrm{c}}}{R_{\mathrm{s}}} = \left(\frac{1}{\phi_{\mathrm{c}}}\right)^{1/3} $$

## Interpreting the Model

This formula shows that the ratio of the cloud radius to the original sphere radius depends on the cube root of the reciprocal of the packing density. Since $ \phi_ {\mathrm{c}} < 1 $ (the debris cannot pack as efficiently as the original solid), we confirm that $ R_ {\mathrm{c}} > R_ {\mathrm{s}} $ as expected.

The exact value of $\phi_{\mathrm{c}}$ would depend on:

-   The shape of the PID pieces
-   Their size distribution
-   The dynamics of the fragmentation process
-   Any forces causing the pieces to separate further

For typical random packing of small fragments, $\phi_{\mathrm{c}}$ might range from $0.3$ to $0.6$, giving values of $\tfrac{R_{\mathrm{c}}}{R_{\mathrm{s}}}$ between approximately $1.2$ and $1.5$.

This model provides a physically meaningful relationship between the two radii based on fundamental principles of mass conservation and packing geometry.
