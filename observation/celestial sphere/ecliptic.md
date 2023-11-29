---
title: Ecliptic
layout: default
parent: Celestial Sphere
grand_parent: Observation
nav_order: 3
---

## Ecliptic Coordinate System

In astronomy, the ecliptic coordinate system is a celestial coordinate system commonly used for representing the apparent positions, orbits, and [pole orientations](https://en.wikipedia.org/wiki/Poles_of_astronomical_bodies) of Solar System objects. Because most planets (except Mercury) and many small Solar System bodies have orbits with only slight inclinations to the [ecliptic](#ecliptic), using it as the fundamental plane is convenient.

The system's origin can be the center of either the Sun or Earth, its [primary direction](#primary-direction) is towards the [vernal equinox](./equatorial.md#vernal-equinox), and it has a right-hand convention. It may be implemented in [spherical](#spherical-coordinates) or [rectangular coordinates](#rectangular-coordinates).

The following diagram shows the Ecliptic Coordinate System (Credits: [University of Houston-Clear Lake](https://sceweb.sce.uhcl.edu/helm/WEB-Positional%20Astronomy/Tutorial/Ecliptic%20coordinates/Ecliptic%20coordinates.html)):

<br />

![Ecliptic Coordinate Sphere](<../../assets/images/observation/celestial sphere/ecliptic/sphere.png>)

### Ecliptic

The ecliptic or ecliptic plane is the orbital plane of Earth around the Sun. From the perspective of an observer on Earth, the Sun's movement around the celestial sphere over the course of a year traces out a path along the ecliptic against the background of stars. The ecliptic is an important reference plane and is the basis of the [ecliptic coordinate system](#ecliptic-coordinate-system).

### Primary Direction

The [celestial equator](./equatorial.md#equator) and the [ecliptic](#ecliptic) are slowly moving due to perturbing forces on the Earth, therefore the orientation of the primary direction, their intersection at the Northern Hemisphere vernal equinox, is not quite fixed. A slow motion of Earth's axis, [precession](./equatorial.md#precession), causes a slow, continuous turning of the coordinate system westward about the poles of the ecliptic, completing one circuit in about 26,000 years. Superimposed on this is a smaller motion of the ecliptic, and a small oscillation of the Earth's axis, [nutation](https://en.wikipedia.org/wiki/Astronomical_nutation).

### Spherical Coordinates

#### Ecliptic Longitude

Ecliptic longitude or celestial longitude (symbol: l) measures the angular distance of an object along the ecliptic from the [primary direction](#primary-direction). Like [right ascension](./equatorial.md#right-ascension) in the equatorial coordinate system, the primary direction (0° ecliptic longitude) points from the Earth towards the Sun at the [vernal equinox](./equatorial.md#vernal-equinox) of the Northern Hemisphere. Because it is a right-handed system, ecliptic longitude is measured positive eastwards in the fundamental plane (the ecliptic) from 0° to 360°.

#### Ecliptic Latitude

Ecliptic latitude (symbol: b), measures the angular distance of an object from the [ecliptic](#ecliptic) towards the north (positive) or south (negative) ecliptic pole. Eg., the north ecliptic pole has a celestial latitude of +90°. Ecliptic latitude for "fixed stars" is not affected by [precession](./equatorial.md#precession).

#### Distance

Distance is also necessary for a complete spherical position (symbol: r). Different distance units are used for different objects. Within the Solar System, [astronomical units](https://en.wikipedia.org/wiki/Astronomical_unit) are used, and for objects near the Earth, Earth radii or kilometers are used.

{: .fun}

> From antiquity through the 18th century, [ecliptic longitude](#ecliptic-longitude) was commonly measured using twelve zodiacal signs, each of 30° longitude, a practice that continues in modern astrology. The signs approximately corresponded to the constellations crossed by the [ecliptic](#ecliptic).

### Rectangular Coordinates

A rectangular variant of ecliptic coordinates is often used in orbital calculations and simulations. It has its origin at the center of the Sun (or at the barycenter of the Solar System), its fundamental plane on the ecliptic plane, and the x-axis toward the [vernal equinox](./equatorial.md#vernal-equinox). The coordinates have a right-handed convention, that is, if one extends their right thumb upward, it simulates the z-axis, their extended index finger the x-axis, and the curl of the other fingers points generally in the direction of the y-axis.

These rectangular coordinates are related to the corresponding spherical coordinates by:

- x = r cos b cos l
- y = r cos b sin l
- z = r sin b

### Conversion between celestial coordinate systems

#### Conversion from ecliptic coordinates to equatorial coordinates

<!-- $$
\begin{equation}
\left(\begin{array}{cc} 
x_{equatorial}\\ 
y_{equatorial}\\ 
z_{equatorial} 
\end{array}\right) =
\left(\begin{array}{cc} 
1 & 0 & 0\\ 
0 & cos ε & -sin ε\\
0 & sin ε & cos ε
\end{array}\right)
\left(\begin{array}{cc} 
x_{ecliptic}\\ 
y_{ecliptic}\\ 
z_{ecliptic} 
\end{array}\right)
\end{equation}
$$ -->

<br />

![Coordinate Conversion](<../../assets/images/observation/celestial sphere/ecliptic/1.png>)

where: 

- $$ε$$ = obliquity of the ecliptic