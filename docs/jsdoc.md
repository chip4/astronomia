## Modules

<dl>
<dt><a href="#module_angle">angle</a></dt>
<dd></dd>
<dt><a href="#module_apparent">apparent</a></dt>
<dd></dd>
<dt><a href="#module_apsis">apsis</a></dt>
<dd></dd>
<dt><a href="#module_base">base</a></dt>
<dd></dd>
<dt><a href="#module_binary">binary</a></dt>
<dd></dd>
<dt><a href="#module_circle">circle</a></dt>
<dd></dd>
<dt><a href="#module_conjunction">conjunction</a></dt>
<dd></dd>
<dt><a href="#module_coord">coord</a></dt>
<dd></dd>
<dt><a href="#module_deltat">deltat</a></dt>
<dd></dd>
<dt><a href="#module_eclipse">eclipse</a></dt>
<dd></dd>
<dt><a href="#module_elementequinox">elementequinox</a></dt>
<dd></dd>
<dt><a href="#module_elliptic">elliptic</a></dt>
<dd></dd>
<dt><a href="#module_eqtime">eqtime</a></dt>
<dd></dd>
<dt><a href="#module_fit">fit</a></dt>
<dd></dd>
<dt><a href="#module_globe">globe</a></dt>
<dd></dd>
<dt><a href="#module_illum">illum</a></dt>
<dd></dd>
<dt><a href="#module_interpolation">interpolation</a></dt>
<dd></dd>
<dt><a href="#module_iterate">iterate</a></dt>
<dd></dd>
<dt><a href="#module_jm">jm</a></dt>
<dd></dd>
<dt><a href="#module_julian">julian</a></dt>
<dd></dd>
<dt><a href="#module_jupiter">jupiter</a></dt>
<dd></dd>
<dt><a href="#module_jupitermoons">jupitermoons</a></dt>
<dd></dd>
<dt><a href="#module_kepler">kepler</a></dt>
<dd></dd>
<dt><a href="#module_line">line</a></dt>
<dd></dd>
<dt><a href="#module_mars">mars</a></dt>
<dd></dd>
<dt><a href="#module_moon">moon</a></dt>
<dd></dd>
<dt><a href="#module_moonillum">moonillum</a></dt>
<dd></dd>
<dt><a href="#module_moonmaxdec">moonmaxdec</a></dt>
<dd></dd>
<dt><a href="#module_moonnode">moonnode</a></dt>
<dd></dd>
<dt><a href="#module_moonphase">moonphase</a></dt>
<dd></dd>
<dt><a href="#module_moonposition">moonposition</a></dt>
<dd></dd>
<dt><a href="#module_nearparabolic">nearparabolic</a></dt>
<dd></dd>
<dt><a href="#module_node">node</a></dt>
<dd></dd>
<dt><a href="#module_nutation">nutation</a></dt>
<dd></dd>
<dt><a href="#module_parabolic">parabolic</a></dt>
<dd></dd>
<dt><a href="#module_parallactic">parallactic</a></dt>
<dd></dd>
<dt><a href="#module_parallax">parallax</a></dt>
<dd></dd>
<dt><a href="#module_perihelion">perihelion</a></dt>
<dd></dd>
<dt><a href="#module_planetary">planetary</a></dt>
<dd></dd>
<dt><a href="#module_planetelements">planetelements</a></dt>
<dd></dd>
<dt><a href="#module_planetposition">planetposition</a></dt>
<dd></dd>
<dt><a href="#module_pluto">pluto</a></dt>
<dd></dd>
<dt><a href="#module_precess">precess</a></dt>
<dd></dd>
<dt><a href="#module_refraction">refraction</a></dt>
<dd></dd>
<dt><a href="#module_rise">rise</a></dt>
<dd></dd>
<dt><a href="#module_saturnmoons">saturnmoons</a></dt>
<dd></dd>
<dt><a href="#module_saturnring">saturnring</a></dt>
<dd></dd>
<dt><a href="#module_semidiameter">semidiameter</a></dt>
<dd></dd>
<dt><a href="#module_sexagesimal">sexagesimal</a></dt>
<dd></dd>
<dt><a href="#module_sidereal">sidereal</a></dt>
<dd></dd>
<dt><a href="#module_solar">solar</a></dt>
<dd></dd>
<dt><a href="#module_solardisk">solardisk</a></dt>
<dd></dd>
<dt><a href="#module_solarxyz">solarxyz</a></dt>
<dd></dd>
<dt><a href="#module_solstice">solstice</a></dt>
<dd></dd>
<dt><a href="#module_stellar">stellar</a></dt>
<dd></dd>
<dt><a href="#module_sundial">sundial</a></dt>
<dd></dd>
<dt><a href="#module_sunrise">sunrise</a></dt>
<dd></dd>
<dt><a href="#module_vsop87">vsop87</a></dt>
<dd></dd>
</dl>

## Classes

<dl>
<dt><a href="#Planet">Planet</a></dt>
<dd></dd>
</dl>

<a name="module_angle"></a>

## angle
**License**: MIT  
**Copyright**: 2016 commenthol  

* [angle](#module_angle)
    * [.sep(c1, c2)](#module_angle.sep) ⇒ <code>Number</code>
    * [.minSep(jd1, jd3, cs1, cs2, [fnSep])](#module_angle.minSep) ⇒ <code>Number</code>
    * [.minSepRect(jd1, jd3, cs1, cs2)](#module_angle.minSepRect) ⇒ <code>Number</code>
    * [.hav()](#module_angle.hav)
    * [.sepHav(c1, c2)](#module_angle.sepHav) ⇒ <code>Number</code>
    * [.minSepHav()](#module_angle.minSepHav)
    * [.sepPauwels(c1, c2)](#module_angle.sepPauwels) ⇒ <code>Number</code>
    * [.minSepPauwels()](#module_angle.minSepPauwels)
    * [.relativePosition(c1, c2)](#module_angle.relativePosition) ⇒ <code>Number</code>

<a name="module_angle.sep"></a>

### angle.sep(c1, c2) ⇒ <code>Number</code>
`sep` returns the angular separation between two celestial bodies.

The algorithm is numerically naïve, and while patched up a bit for
small separations, remains unstable for separations near π.

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - angular separation between two celestial bodies  

| Param | Type | Description |
| --- | --- | --- |
| c1 | <code>base.Coord</code> | coordinate of celestial body 1 |
| c2 | <code>base.Coord</code> | coordinate of celestial body 2 |

<a name="module_angle.minSep"></a>

### angle.minSep(jd1, jd3, cs1, cs2, [fnSep]) ⇒ <code>Number</code>
`minSep` returns the minimum separation between two moving objects.

The motion is represented as an ephemeris of three rows, equally spaced
in time.  Jd1, jd3 are julian day times of the first and last rows.
R1, d1, r2, d2 are coordinates at the three times.  They must each be
slices of length 3.0

Result is obtained by computing separation at each of the three times
and interpolating a minimum.  This may be invalid for sufficiently close
approaches.

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - angular separation between two celestial bodies  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| jd1 | <code>Number</code> | Julian day - time at cs1[0], cs2[0] |
| jd3 | <code>Number</code> | Julian day - time at cs1[2], cs2[2] |
| cs1 | <code>Array.&lt;base.Coord&gt;</code> | 3 coordinates of moving object 1 |
| cs2 | <code>Array.&lt;base.Coord&gt;</code> | 3 coordinates of moving object 2 |
| [fnSep] | <code>function</code> | alternative `sep` function e.g. `angle.sepPauwels`, `angle.sepHav` |

<a name="module_angle.minSepRect"></a>

### angle.minSepRect(jd1, jd3, cs1, cs2) ⇒ <code>Number</code>
`minSepRect` returns the minimum separation between two moving objects.

Like `minSep`, but using a method of rectangular coordinates that gives
accurate results even for close approaches.

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - angular separation between two celestial bodies  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| jd1 | <code>Number</code> | Julian day - time at cs1[0], cs2[0] |
| jd3 | <code>Number</code> | Julian day - time at cs1[2], cs2[2] |
| cs1 | <code>Array.&lt;base.Coord&gt;</code> | 3 coordinates of moving object 1 |
| cs2 | <code>Array.&lt;base.Coord&gt;</code> | 3 coordinates of moving object 2 |

<a name="module_angle.hav"></a>

### angle.hav()
haversine function (17.5) p. 115

**Kind**: static method of [<code>angle</code>](#module_angle)  
<a name="module_angle.sepHav"></a>

### angle.sepHav(c1, c2) ⇒ <code>Number</code>
`sepHav` returns the angular separation between two celestial bodies.

The algorithm uses the haversine function and is superior to the naïve
algorithm of the Sep function.

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - angular separation between two celestial bodies  

| Param | Type | Description |
| --- | --- | --- |
| c1 | <code>base.Coord</code> | coordinate of celestial body 1 |
| c2 | <code>base.Coord</code> | coordinate of celestial body 2 |

<a name="module_angle.minSepHav"></a>

### angle.minSepHav()
Same as `minSep` but uses function `sepHav` to return the minimum separation
between two moving objects.

**Kind**: static method of [<code>angle</code>](#module_angle)  
<a name="module_angle.sepPauwels"></a>

### angle.sepPauwels(c1, c2) ⇒ <code>Number</code>
`sepPauwels` returns the angular separation between two celestial bodies.

The algorithm is a numerically stable form of that used in `sep`.

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - angular separation between two celestial bodies  

| Param | Type | Description |
| --- | --- | --- |
| c1 | <code>base.Coord</code> | coordinate of celestial body 1 |
| c2 | <code>base.Coord</code> | coordinate of celestial body 2 |

<a name="module_angle.minSepPauwels"></a>

### angle.minSepPauwels()
Same as `minSep` but uses function `sepPauwels` to return the minimum
separation between two moving objects.

**Kind**: static method of [<code>angle</code>](#module_angle)  
<a name="module_angle.relativePosition"></a>

### angle.relativePosition(c1, c2) ⇒ <code>Number</code>
RelativePosition returns the position angle of one body with respect to
another.

The position angle result `p` is measured counter-clockwise from North.
If negative then `p` is in the range of 90° ... 270°

````
                 North
                   |
            (p)  ..|
                .  |
               V   |
   c1 x------------x c2
                   |
````

**Kind**: static method of [<code>angle</code>](#module_angle)  
**Returns**: <code>Number</code> - position angle (p)  

| Param | Type | Description |
| --- | --- | --- |
| c1 | <code>base.Coord</code> | coordinate of celestial body 1 |
| c2 | <code>base.Coord</code> | coordinate of celestial body 2 |

<a name="module_apparent"></a>

## apparent
**License**: MIT  
**Copyright**: 2016 commenthol  

* [apparent](#module_apparent)
    * _static_
        * [.nutation(α, δ, jd)](#module_apparent.nutation) ⇒ <code>Array.&lt;Number&gt;</code>
        * [.perihelion()](#module_apparent.perihelion)
        * [.eclipticAberration()](#module_apparent.eclipticAberration)
        * [.aberration()](#module_apparent.aberration)
        * [.position()](#module_apparent.position)
        * [.aberrationRonVondrak()](#module_apparent.aberrationRonVondrak)
        * [.positionRonVondrak()](#module_apparent.positionRonVondrak)
    * _inner_
        * [~κ](#module_apparent..κ)

<a name="module_apparent.nutation"></a>

### apparent.nutation(α, δ, jd) ⇒ <code>Array.&lt;Number&gt;</code>
Nutation returns corrections due to nutation for equatorial coordinates
of an object.

Results are invalid for objects very near the celestial poles.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
**Returns**: <code>Array.&lt;Number&gt;</code> - [Δα1, Δδ1] -  

| Param | Type | Description |
| --- | --- | --- |
| α | <code>Number</code> | right ascension |
| δ | <code>Number</code> | declination |
| jd | <code>Number</code> | Julian Day |

<a name="module_apparent.perihelion"></a>

### apparent.perihelion()
longitude of perihelian of Earth's orbit.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent.eclipticAberration"></a>

### apparent.eclipticAberration()
EclipticAberration returns corrections due to aberration for ecliptic
coordinates of an object.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent.aberration"></a>

### apparent.aberration()
Aberration returns corrections due to aberration for equatorial
coordinates of an object.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent.position"></a>

### apparent.position()
Position computes the apparent position of an object.

Position is computed for equatorial coordinates in eqFrom, considering
proper motion, precession, nutation, and aberration.  Result is in
eqTo.  EqFrom and eqTo must be non-nil, but may point to the same struct.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent.aberrationRonVondrak"></a>

### apparent.aberrationRonVondrak()
AberrationRonVondrak uses the Ron-Vondrák expression to compute corrections
due to aberration for equatorial coordinates of an object.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent.positionRonVondrak"></a>

### apparent.positionRonVondrak()
PositionRonVondrak computes the apparent position of an object using
the Ron-Vondrák expression for aberration.

Position is computed for equatorial coordinates in eqFrom, considering
proper motion, aberration, precession, and _nutation.  Result is in
eqTo.  EqFrom and eqTo must be non-nil, but may point to the same struct.

Note the Ron-Vondrák expression is only valid for the epoch J2000.
EqFrom must be coordinates at epoch J2000.

**Kind**: static method of [<code>apparent</code>](#module_apparent)  
<a name="module_apparent..κ"></a>

### apparent~κ
κ is the constant of aberration in radians.

**Kind**: inner constant of [<code>apparent</code>](#module_apparent)  
<a name="module_apsis"></a>

## apsis
**License**: MIT  
**Copyright**: 2016 commenthol  

* [apsis](#module_apsis)
    * _static_
        * [.meanPerigee(year)](#module_apsis.meanPerigee) ⇒ <code>Number</code>
        * [.perigee(year)](#module_apsis.perigee) ⇒ <code>Number</code>
        * [.meanApogee(year)](#module_apsis.meanApogee) ⇒ <code>Number</code>
        * [.apogee(year)](#module_apsis.apogee) ⇒ <code>Number</code>
        * [.apogeeParallax(year)](#module_apsis.apogeeParallax) ⇒ <code>Number</code>
        * [.perigeeParallax(year)](#module_apsis.perigeeParallax) ⇒ <code>Number</code>
        * [.distance(parallax)](#module_apsis.distance) ⇒ <code>Number</code>
    * _inner_
        * [~ck](#module_apsis..ck)
        * [~mean()](#module_apsis..mean)
        * [~snap()](#module_apsis..snap)

<a name="module_apsis.meanPerigee"></a>

### apsis.meanPerigee(year) ⇒ <code>Number</code>
meanPerigee returns the jde of the mean perigee of the Moon nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.perigee"></a>

### apsis.perigee(year) ⇒ <code>Number</code>
perigee returns the jde of perigee of the Moon nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.meanApogee"></a>

### apsis.meanApogee(year) ⇒ <code>Number</code>
meanApogee returns the jde of the mean apogee of the Moon nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.apogee"></a>

### apsis.apogee(year) ⇒ <code>Number</code>
apogee returns the jde of apogee of the Moon nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.apogeeParallax"></a>

### apsis.apogeeParallax(year) ⇒ <code>Number</code>
apogeeParallax returns equatorial horizontal parallax of the Moon at the Apogee nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - equatorial horizontal parallax in radians  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.perigeeParallax"></a>

### apsis.perigeeParallax(year) ⇒ <code>Number</code>
perigeeParallax returns equatorial horizontal parallax of the Moon at the Apogee nearest the given date.

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - equatorial horizontal parallax in radians  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying a date. |

<a name="module_apsis.distance"></a>

### apsis.distance(parallax) ⇒ <code>Number</code>
Calculate the distance earth - moon (center to center) using the parallax angle in radians

**Kind**: static method of [<code>apsis</code>](#module_apsis)  
**Returns**: <code>Number</code> - distance in `km`  

| Param | Type | Description |
| --- | --- | --- |
| parallax | <code>Number</code> | parallax angle in radians |

<a name="module_apsis..ck"></a>

### apsis~ck
conversion factor from k to T, given in (50.3) p. 356

**Kind**: inner constant of [<code>apsis</code>](#module_apsis)  
<a name="module_apsis..mean"></a>

### apsis~mean()
mean time of perigee or apogee
(50.1) p. 355

**Kind**: inner method of [<code>apsis</code>](#module_apsis)  
<a name="module_apsis..snap"></a>

### apsis~snap()
snap returns k at half h nearest year y.

**Kind**: inner method of [<code>apsis</code>](#module_apsis)  
<a name="module_base"></a>

## base
**License**: MIT  
**Copyright**: 2016 commenthol  

* [base](#module_base)
    * [.K](#module_base.K)
    * [.AU](#module_base.AU)
    * [.SOblJ2000](#module_base.SOblJ2000)
    * [.COblJ2000](#module_base.COblJ2000)
    * [.JMod](#module_base.JMod)
    * [.J2000](#module_base.J2000)
    * [.J1900](#module_base.J1900)
    * [.B1900](#module_base.B1900)
    * [.B1950](#module_base.B1950)
    * [.JulianYear](#module_base.JulianYear)
    * [.JulianCentury](#module_base.JulianCentury)
    * [.BesselianYear](#module_base.BesselianYear)
    * [.meanSiderealYear](#module_base.meanSiderealYear)
    * [.SmallAngle](#module_base.SmallAngle)
    * [.CosSmallAngle](#module_base.CosSmallAngle)
    * [.lightTime(dist)](#module_base.lightTime) ⇒ <code>Number</code>
    * [.JulianYearToJDE(jy)](#module_base.JulianYearToJDE) ⇒ <code>Number</code>
    * [.JDEToJulianYear(jde)](#module_base.JDEToJulianYear) ⇒ <code>Number</code>
    * [.BesselianYearToJDE(by)](#module_base.BesselianYearToJDE) ⇒ <code>Number</code>
    * [.JDEToBesselianYear(jde)](#module_base.JDEToBesselianYear) ⇒ <code>Number</code>
    * [.J2000Century(jde)](#module_base.J2000Century) ⇒ <code>Number</code>
    * [.illuminated(i)](#module_base.illuminated) ⇒ <code>Number</code>
    * [.Coord(ra, dec, [range], [elongation])](#module_base.Coord)
    * [.limb(equ, appSun)](#module_base.limb) ⇒ <code>Number</code>
    * [.pmod(x, y)](#module_base.pmod) ⇒ <code>Number</code>
    * [.horner(x, c)](#module_base.horner) ⇒ <code>Number</code>
    * [.floorDiv(x, y)](#module_base.floorDiv) ⇒ <code>Number</code>
    * [.cmp(a, b)](#module_base.cmp) ⇒ <code>Number</code>
    * [.sincos(ε)](#module_base.sincos) ⇒ <code>Array.&lt;Number&gt;</code>
    * [.toRad(deg)](#module_base.toRad) ⇒ <code>Number</code>
    * [.toDeg(rad)](#module_base.toDeg) ⇒ <code>Number</code>
    * [.modf(float)](#module_base.modf) ⇒ <code>Array</code>
    * [.round(float, precision)](#module_base.round) ⇒ <code>Number</code>

<a name="module_base.K"></a>

### base.K
K is the Gaussian gravitational constant.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.AU"></a>

### base.AU
AU is one astronomical unit in km.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.SOblJ2000"></a>

### base.SOblJ2000
SOblJ2000 sine obliquity at J2000.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.COblJ2000"></a>

### base.COblJ2000
COblJ2000 cosine obliquity at J2000.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.JMod"></a>

### base.JMod
JMod is the Julian date of the modified Julian date epoch.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.J2000"></a>

### base.J2000
J2000 is the Julian date corresponding to January 1.5, year 2000.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.J1900"></a>

### base.J1900
Julian days of Julian epoch 1900

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.B1900"></a>

### base.B1900
Julian days of Besselian epoch 1900

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.B1950"></a>

### base.B1950
Julian days of Besselian epoch 1950

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.JulianYear"></a>

### base.JulianYear
JulianYear in days

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.JulianCentury"></a>

### base.JulianCentury
JulianCentury in days

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.BesselianYear"></a>

### base.BesselianYear
BesselianYear in days; equals mean tropical year

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.meanSiderealYear"></a>

### base.meanSiderealYear
Mean sidereal year

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.SmallAngle"></a>

### base.SmallAngle
SmallAngle is threshold used by various routines for switching between
trigonometric functions and Pythagorean approximations.

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.CosSmallAngle"></a>

### base.CosSmallAngle
cosine of SmallAngle

**Kind**: static constant of [<code>base</code>](#module_base)  
<a name="module_base.lightTime"></a>

### base.lightTime(dist) ⇒ <code>Number</code>
lightTime returns time for light to travel a given distance.
`dist` is distance in to earth in AU. √(x² + y² + z²)
Result in seconds of time.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - time for light to travel a given distance in seconds  

| Param | Type | Description |
| --- | --- | --- |
| dist | <code>Number</code> | distance in to earth in AU |

<a name="module_base.JulianYearToJDE"></a>

### base.JulianYearToJDE(jy) ⇒ <code>Number</code>
JulianYearToJDE returns the Julian ephemeris day for a Julian year.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| jy | <code>Number</code> | Julian year |

<a name="module_base.JDEToJulianYear"></a>

### base.JDEToJulianYear(jde) ⇒ <code>Number</code>
JDEToJulianYear returns a Julian year for a Julian ephemeris day.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - jy - Julian year  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_base.BesselianYearToJDE"></a>

### base.BesselianYearToJDE(by) ⇒ <code>Number</code>
BesselianYearToJDE returns the Julian ephemeris day for a Besselian year.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - jde - Julian ephemeris day  

| Param | Type | Description |
| --- | --- | --- |
| by | <code>Number</code> | Besselian year |

<a name="module_base.JDEToBesselianYear"></a>

### base.JDEToBesselianYear(jde) ⇒ <code>Number</code>
JDEToBesselianYear returns the Besselian year for a Julian ephemeris day.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - by - Besselian year  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_base.J2000Century"></a>

### base.J2000Century(jde) ⇒ <code>Number</code>
J2000Century returns the number of Julian centuries since J2000.

The quantity appears as T in a number of time series.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - number of Julian centuries since J2000  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_base.illuminated"></a>

### base.illuminated(i) ⇒ <code>Number</code>
illuminated returns the illuminated fraction of a body's disk.

The illuminated body can be the Moon or a planet.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - illuminated fraction of a body's disk.  

| Param | Type | Description |
| --- | --- | --- |
| i | <code>Number</code> | phase angle in radians. |

<a name="module_base.Coord"></a>

### base.Coord(ra, dec, [range], [elongation])
celestial coordinates in right ascension and declination
or ecliptic coordinates in longitude and latitude

**Kind**: static method of [<code>base</code>](#module_base)  

| Param | Type | Description |
| --- | --- | --- |
| ra | <code>number</code> | right ascension (or longitude) |
| dec | <code>number</code> | declination (or latitude) |
| [range] | <code>number</code> | distance |
| [elongation] | <code>number</code> | elongation |

<a name="module_base.limb"></a>

### base.limb(equ, appSun) ⇒ <code>Number</code>
Limb returns the position angle of the midpoint of an illuminated limb.

The illuminated body can be the Moon or a planet.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - position angle of the midpoint (in radians).  

| Param | Type | Description |
| --- | --- | --- |
| equ | <code>base.Coord</code> | equatorial coordinates of the body `{ra, dec}` (in radians) |
| appSun | <code>base.Coord</code> | apparent coordinates of the Sun `{ra, dec}` (In radians). |

<a name="module_base.pmod"></a>

### base.pmod(x, y) ⇒ <code>Number</code>
pmod returns a positive floating-point x mod y.

For a positive argument y, it returns a value in the range [0,y).

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - x % y - The result may not be useful if y is negative.  

| Param | Type |
| --- | --- |
| x | <code>Number</code> | 
| y | <code>Number</code> | 

<a name="module_base.horner"></a>

### base.horner(x, c) ⇒ <code>Number</code>
horner evaluates a polynomal with coefficients c at x.  The constant
term is c[0].

**Kind**: static method of [<code>base</code>](#module_base)  

| Param | Type | Description |
| --- | --- | --- |
| x | <code>Number</code> |  |
| c | <code>Number</code> \| <code>Array.&lt;Number&gt;</code> | coefficients |

<a name="module_base.floorDiv"></a>

### base.floorDiv(x, y) ⇒ <code>Number</code>
FloorDiv returns the integer floor of the fractional value (x / y).

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - (int)  

| Param | Type |
| --- | --- |
| x | <code>Number</code> | 
| y | <code>Number</code> | 

<a name="module_base.cmp"></a>

### base.cmp(a, b) ⇒ <code>Number</code>
Cmp compares two float64s and returns -1, 0, or 1 if a is <, ==, or > b,
respectively.
.

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - comparison result  

| Param | Type |
| --- | --- |
| a | <code>Number</code> | 
| b | <code>Number</code> | 

<a name="module_base.sincos"></a>

### base.sincos(ε) ⇒ <code>Array.&lt;Number&gt;</code>
shorthand function for Math.sin, Math.cos

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Array.&lt;Number&gt;</code> - [sin(ε), cos(ε)]  

| Param | Type |
| --- | --- |
| ε | <code>Number</code> | 

<a name="module_base.toRad"></a>

### base.toRad(deg) ⇒ <code>Number</code>
Convert degrees to radians

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - Angle in radians  

| Param | Type | Description |
| --- | --- | --- |
| deg | <code>Number</code> | Angle in degrees |

<a name="module_base.toDeg"></a>

### base.toDeg(rad) ⇒ <code>Number</code>
Convert radians to degrees

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - Angle in degrees  

| Param | Type | Description |
| --- | --- | --- |
| rad | <code>Number</code> | Angle in radians |

<a name="module_base.modf"></a>

### base.modf(float) ⇒ <code>Array</code>
separate fix `i` from fraction `f`

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Array</code> - [i, f]
 {Number} i - (int) fix value
 {Number} f - (float) fractional portion; always > 1  

| Param | Type |
| --- | --- |
| float | <code>Number</code> | 

<a name="module_base.round"></a>

### base.round(float, precision) ⇒ <code>Number</code>
Rounds `float` value by precision

**Kind**: static method of [<code>base</code>](#module_base)  
**Returns**: <code>Number</code> - rounded `float`  

| Param | Type | Description |
| --- | --- | --- |
| float | <code>Number</code> | value to round |
| precision | <code>Number</code> | (int) number of post decimal positions |

<a name="module_binary"></a>

## binary
**License**: MIT  
**Copyright**: 2016 commenthol  

* [binary](#module_binary)
    * [.meanAnomaly(year, T, P)](#module_binary.meanAnomaly) ⇒ <code>Number</code>
    * [.position(a, e, i, Ω, ω, E)](#module_binary.position) ⇒ <code>Array.&lt;Number&gt;</code>
    * [.apparentEccentricity(e, i, ω)](#module_binary.apparentEccentricity) ⇒ <code>Number</code>

<a name="module_binary.meanAnomaly"></a>

### binary.meanAnomaly(year, T, P) ⇒ <code>Number</code>
computes mean anomaly for the given date.

**Kind**: static method of [<code>binary</code>](#module_binary)  
**Returns**: <code>Number</code> - mean anomaly in radians.  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | is a decimal year specifying the date |
| T | <code>Number</code> | is time of periastron, as a decimal year |
| P | <code>Number</code> | is period of revolution in mean solar years |

<a name="module_binary.position"></a>

### binary.position(a, e, i, Ω, ω, E) ⇒ <code>Array.&lt;Number&gt;</code>
Position computes apparent position angle and angular distance of
components of a binary star.

**Kind**: static method of [<code>binary</code>](#module_binary)  
**Returns**: <code>Array.&lt;Number&gt;</code> - [θ, ρ]
 {Number} θ -is the apparent position angle in radians,
 {Number} ρ is the angular distance in arc seconds.  

| Param | Type | Description |
| --- | --- | --- |
| a | <code>Number</code> | is apparent semimajor axis in arc seconds |
| e | <code>Number</code> | is eccentricity of the true orbit |
| i | <code>Number</code> | is inclination relative to the line of sight |
| Ω | <code>Number</code> | is position angle of the ascending node |
| ω | <code>Number</code> | is longitude of periastron |
| E | <code>Number</code> | is eccentric anomaly, computed for example with package kepler  and the mean anomaly as returned by function M in this package. |

<a name="module_binary.apparentEccentricity"></a>

### binary.apparentEccentricity(e, i, ω) ⇒ <code>Number</code>
ApparentEccentricity returns apparent eccenticity of a binary star
given true orbital elements.

**Kind**: static method of [<code>binary</code>](#module_binary)  
**Returns**: <code>Number</code> - apparent eccenticity of a binary star  

| Param | Type | Description |
| --- | --- | --- |
| e | <code>Number</code> | is eccentricity of the true orbit |
| i | <code>Number</code> | is inclination relative to the line of sight |
| ω | <code>Number</code> | is longitude of periastron |

<a name="module_circle"></a>

## circle
**License**: MIT  
**Copyright**: 2016 commenthol  

* [circle](#module_circle)
    * _static_
        * [.smallest(c1, c2, c3)](#module_circle.smallest) ⇒ <code>Array</code>
    * _inner_
        * [~hav()](#module_circle..hav)

<a name="module_circle.smallest"></a>

### circle.smallest(c1, c2, c3) ⇒ <code>Array</code>
Smallest finds the smallest circle containing three points.

Arguments should represent coordinates in right ascension and declination
or longitude and latitude.  Result Δ is the diameter of the circle, typeI
is true if solution is of type I.

**Kind**: static method of [<code>circle</code>](#module_circle)  
**Returns**: <code>Array</code> - [Δ, typeI]
 {Number} Δ - diameter of the circle
 {Number} typeI - true - Two points on circle, one interior.
                  false - All three points on circle.  

| Param | Type | Description |
| --- | --- | --- |
| c1 | <code>base.Coords</code> | ra, dec point 1 |
| c2 | <code>base.Coords</code> | ra, dec point 2 |
| c3 | <code>base.Coords</code> | ra, dec point 3 |

<a name="module_circle..hav"></a>

### circle~hav()
haversine function (17.5) p. 115

**Kind**: inner method of [<code>circle</code>](#module_circle)  
<a name="module_conjunction"></a>

## conjunction
**License**: MIT  
**Copyright**: 2016 commenthol  

* [conjunction](#module_conjunction)
    * [.planetary(t1, t5, cs1, cs2)](#module_conjunction.planetary) ⇒ <code>Array</code>
    * [.stellar(t1, t5, c1, cs2)](#module_conjunction.stellar) ⇒ <code>Array</code>

<a name="module_conjunction.planetary"></a>

### conjunction.planetary(t1, t5, cs1, cs2) ⇒ <code>Array</code>
Planetary computes a conjunction between two moving objects, such as planets.

Conjunction is found with interpolation against length 5 ephemerides.

t1, t5 are times of first and last rows of ephemerides.  The scale is
arbitrary.

cs1 is the ephemeris of the first object. The columns may be celestial
coordinates in right ascension and declination or ecliptic coordinates in
longitude and latitude.

cs2 is the ephemeris of the second object, in the same frame as the first.

Return value t is time of conjunction in the scale of t1, t5.

**Kind**: static method of [<code>conjunction</code>](#module_conjunction)  
**Returns**: <code>Array</code> - {Number} t - time of conjunction in JDE
   {Number} Δd - is the amount that object 2 was "above" object 1 at the time of conjunction.  

| Param | Type | Description |
| --- | --- | --- |
| t1 | <code>Number</code> | julian ephemeris day of first row |
| t5 | <code>Number</code> | julian ephemeris day of fifth row |
| cs1 | <code>Array.&lt;base.Coord&gt;</code> | ephemeris of first moving object |
| cs2 | <code>Array.&lt;base.Coord&gt;</code> | ephemeris of decond moving object |

<a name="module_conjunction.stellar"></a>

### conjunction.stellar(t1, t5, c1, cs2) ⇒ <code>Array</code>
Stellar computes a conjunction between a moving and non-moving object.

Arguments and return values same as with Planetary, except the non-moving
object is c1.  The ephemeris of the moving object is cs2.

**Kind**: static method of [<code>conjunction</code>](#module_conjunction)  
**Returns**: <code>Array</code> - {Number} t - time of conjunction in JDE
   {Number} Δd - is the amount that object 2 was "above" object 1 at the time of conjunction.  

| Param | Type | Description |
| --- | --- | --- |
| t1 | <code>Number</code> | julian ephemeris day of first row |
| t5 | <code>Number</code> | julian ephemeris day of fifth row |
| c1 | <code>base.Coord</code> | ephemeris of non-moving object |
| cs2 | <code>Array.&lt;base.Coord&gt;</code> | ephemeris of moving object |

<a name="module_coord"></a>

## coord
**License**: MIT  
**Copyright**: 2016 commenthol  

* [coord](#module_coord)
    * [.Ecliptic](#module_coord.Ecliptic)
        * [new exports.Ecliptic(lon, lat)](#new_module_coord.Ecliptic_new)
        * [.toEquatorial(ε)](#module_coord.Ecliptic+toEquatorial) ⇒ <code>Equatorial</code>
    * [.Equatorial](#module_coord.Equatorial)
        * [new exports.Equatorial(ra, dec)](#new_module_coord.Equatorial_new)
        * [.toEcliptic(ε)](#module_coord.Equatorial+toEcliptic) ⇒ <code>Ecliptic</code>
        * [.toHorizontal(eq, g, st)](#module_coord.Equatorial+toHorizontal) ⇒ <code>Horizontal</code>
        * [.toGalactic(eq)](#module_coord.Equatorial+toGalactic) ⇒ <code>Galactic</code>
    * [.Horizontal](#module_coord.Horizontal)
        * [new exports.Horizontal(az, alt)](#new_module_coord.Horizontal_new)
        * [.toEquatorial(g, st)](#module_coord.Horizontal+toEquatorial) ⇒ <code>Equatorial</code>
    * [.Galactic](#module_coord.Galactic)
        * [new exports.Galactic(lon, lat)](#new_module_coord.Galactic_new)
        * [.toEquatorial()](#module_coord.Galactic+toEquatorial) ⇒ <code>Equatorial</code>
    * [.galacticNorth](#module_coord.galacticNorth)
    * [.galacticLon0](#module_coord.galacticLon0)

<a name="module_coord.Ecliptic"></a>

### coord.Ecliptic
Ecliptic coordinates are referenced to the plane of the ecliptic.

**Kind**: static class of [<code>coord</code>](#module_coord)  

* [.Ecliptic](#module_coord.Ecliptic)
    * [new exports.Ecliptic(lon, lat)](#new_module_coord.Ecliptic_new)
    * [.toEquatorial(ε)](#module_coord.Ecliptic+toEquatorial) ⇒ <code>Equatorial</code>

<a name="new_module_coord.Ecliptic_new"></a>

#### new exports.Ecliptic(lon, lat)
IMPORTANT: Longitudes are measured *positively* westwards
e.g. Washington D.C. +77°04; Vienna -16°23'


| Param | Type | Description |
| --- | --- | --- |
| lon | <code>Number</code> | Longitude (λ) in radians |
| lat | <code>Number</code> | Latitude (β) in radians |

<a name="module_coord.Ecliptic+toEquatorial"></a>

#### ecliptic.toEquatorial(ε) ⇒ <code>Equatorial</code>
converts ecliptic coordinates to equatorial coordinates.

**Kind**: instance method of [<code>Ecliptic</code>](#module_coord.Ecliptic)  

| Param | Type | Description |
| --- | --- | --- |
| ε | <code>Number</code> | Obliquity |

<a name="module_coord.Equatorial"></a>

### coord.Equatorial
Equatorial coordinates are referenced to the Earth's rotational axis.

**Kind**: static class of [<code>coord</code>](#module_coord)  

* [.Equatorial](#module_coord.Equatorial)
    * [new exports.Equatorial(ra, dec)](#new_module_coord.Equatorial_new)
    * [.toEcliptic(ε)](#module_coord.Equatorial+toEcliptic) ⇒ <code>Ecliptic</code>
    * [.toHorizontal(eq, g, st)](#module_coord.Equatorial+toHorizontal) ⇒ <code>Horizontal</code>
    * [.toGalactic(eq)](#module_coord.Equatorial+toGalactic) ⇒ <code>Galactic</code>

<a name="new_module_coord.Equatorial_new"></a>

#### new exports.Equatorial(ra, dec)

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| ra | <code>Number</code> | <code>0</code> | (float) Right ascension (α) in radians |
| dec | <code>Number</code> | <code>0</code> | (float) Declination (δ) in radians |

<a name="module_coord.Equatorial+toEcliptic"></a>

#### equatorial.toEcliptic(ε) ⇒ <code>Ecliptic</code>
EqToEcl converts equatorial coordinates to ecliptic coordinates.

**Kind**: instance method of [<code>Equatorial</code>](#module_coord.Equatorial)  

| Param | Type | Description |
| --- | --- | --- |
| ε | <code>Number</code> | Obliquity |

<a name="module_coord.Equatorial+toHorizontal"></a>

#### equatorial.toHorizontal(eq, g, st) ⇒ <code>Horizontal</code>
EqToHz computes Horizontal coordinates from equatorial coordinates.

Argument g is the location of the observer on the Earth.  Argument st
is the sidereal time at Greenwich.

Sidereal time must be consistent with the equatorial coordinates.
If coordinates are apparent, sidereal time must be apparent as well.

**Kind**: instance method of [<code>Equatorial</code>](#module_coord.Equatorial)  

| Param | Type | Description |
| --- | --- | --- |
| eq | <code>Equatorial</code> | equatorial coordinates (right ascension, declination) |
| g | <code>globe.Coord</code> | coordinates of observer on Earth |
| st | <code>Number</code> | sidereal time at Greenwich at time of observation |

<a name="module_coord.Equatorial+toGalactic"></a>

#### equatorial.toGalactic(eq) ⇒ <code>Galactic</code>
EqToGal converts equatorial coordinates to galactic coordinates.

Equatorial coordinates must be referred to the standard equinox of B1950.0.
For conversion to B1950, see package precess and utility functions in
package "common".

**Kind**: instance method of [<code>Equatorial</code>](#module_coord.Equatorial)  

| Param | Type |
| --- | --- |
| eq | <code>Equatorial</code> | 

<a name="module_coord.Horizontal"></a>

### coord.Horizontal
Horizontal coordinates are referenced to the local horizon of an observer
on the surface of the Earth.

**Kind**: static class of [<code>coord</code>](#module_coord)  

* [.Horizontal](#module_coord.Horizontal)
    * [new exports.Horizontal(az, alt)](#new_module_coord.Horizontal_new)
    * [.toEquatorial(g, st)](#module_coord.Horizontal+toEquatorial) ⇒ <code>Equatorial</code>

<a name="new_module_coord.Horizontal_new"></a>

#### new exports.Horizontal(az, alt)

| Param | Type | Description |
| --- | --- | --- |
| az | <code>Number</code> | Azimuth (A) in radians |
| alt | <code>Number</code> | Altitude (h) in radians |

<a name="module_coord.Horizontal+toEquatorial"></a>

#### horizontal.toEquatorial(g, st) ⇒ <code>Equatorial</code>
transforms horizontal coordinates to equatorial coordinates.

Sidereal time must be consistent with the equatorial coordinates.
If coordinates are apparent, sidereal time must be apparent as well.

**Kind**: instance method of [<code>Horizontal</code>](#module_coord.Horizontal)  
**Returns**: <code>Equatorial</code> - (right ascension, declination)  

| Param | Type | Description |
| --- | --- | --- |
| g | <code>globe.Coord</code> | coordinates of observer on Earth (lat, lon) |
| st | <code>Number</code> | sidereal time at Greenwich at time of observation. |

<a name="module_coord.Galactic"></a>

### coord.Galactic
Galactic coordinates are referenced to the plane of the Milky Way.

**Kind**: static class of [<code>coord</code>](#module_coord)  

* [.Galactic](#module_coord.Galactic)
    * [new exports.Galactic(lon, lat)](#new_module_coord.Galactic_new)
    * [.toEquatorial()](#module_coord.Galactic+toEquatorial) ⇒ <code>Equatorial</code>

<a name="new_module_coord.Galactic_new"></a>

#### new exports.Galactic(lon, lat)

| Param | Type | Description |
| --- | --- | --- |
| lon | <code>Number</code> | Longitude (l) in radians |
| lat | <code>Number</code> | Latitude (b) in radians |

<a name="module_coord.Galactic+toEquatorial"></a>

#### galactic.toEquatorial() ⇒ <code>Equatorial</code>
GalToEq converts galactic coordinates to equatorial coordinates.

Resulting equatorial coordinates will be referred to the standard equinox of
B1950.0.  For subsequent conversion to other epochs, see package precess and
utility functions in package meeus.

**Kind**: instance method of [<code>Galactic</code>](#module_coord.Galactic)  
**Returns**: <code>Equatorial</code> - (right ascension, declination)  
<a name="module_coord.galacticNorth"></a>

### coord.galacticNorth
equatorial coords for galactic north
IAU B1950.0 coordinates of galactic North Pole

**Kind**: static constant of [<code>coord</code>](#module_coord)  
<a name="module_coord.galacticLon0"></a>

### coord.galacticLon0
Galactic Longitude 0°
Meeus gives 33 as the origin of galactic longitudes relative to the
ascending node of of the galactic equator.  33 + 90 = 123, the IAU
value for origin relative to the equatorial pole.

**Kind**: static constant of [<code>coord</code>](#module_coord)  
<a name="module_deltat"></a>

## deltat
**License**: MIT  
**Copyright**: 2016 commenthol  
<a name="module_deltat.deltaT"></a>

### deltat.deltaT(dyear) ⇒ <code>Number</code>
deltaT returns the difference ΔT = TD - UT between Dynamical Time TD and
Univeral Time (GMT+12) in seconds

Polynoms are from <http://eclipse.gsfc.nasa.gov/SEcat5/deltatpoly.html>
and <http://www.staff.science.uu.nl/~gent0113/deltat/deltat_old.htm>

**Kind**: static method of [<code>deltat</code>](#module_deltat)  
**Returns**: <code>Number</code> - ΔT in seconds.  

| Param | Type | Description |
| --- | --- | --- |
| dyear | <code>Number</code> | decimal year |

<a name="module_eclipse"></a>

## eclipse
**License**: MIT  
**Copyright**: 2016 commenthol  

* [eclipse](#module_eclipse)
    * _static_
        * [.TYPE](#module_eclipse.TYPE)
        * [.solar()](#module_eclipse.solar)
        * [.lunar()](#module_eclipse.lunar)
    * _inner_
        * [~snap()](#module_eclipse..snap)

<a name="module_eclipse.TYPE"></a>

### eclipse.TYPE
Eclipse type identifiers returned from Solar and Lunar.

**Kind**: static constant of [<code>eclipse</code>](#module_eclipse)  
<a name="module_eclipse.solar"></a>

### eclipse.solar()
Solar computes quantities related to solar eclipses.

Argument year is a decimal year specifying a date.

eclipseType will be None, Partial, Annular, AnnularTotal, or Total.
If None, none of the other return values may be meaningful.

central is true if the center of the eclipse shadow touches the Earth.

jdeMax is the jde when the center of the eclipse shadow is closest to the
Earth center, in a plane through the center of the Earth.

γ is the distance from the eclipse shadow center to the Earth center
at time jdeMax.

u is the radius of the Moon's umbral cone in the plane of the Earth.

p is the radius of the penumbral cone.

mag is eclipse magnitude for partial eclipses.  It is not valid for other
eclipse types.

γ, u, and p are in units of equatorial Earth radii.

**Kind**: static method of [<code>eclipse</code>](#module_eclipse)  
<a name="module_eclipse.lunar"></a>

### eclipse.lunar()
Lunar computes quantities related to lunar eclipses.

Argument year is a decimal year specifying a date.

eclipseType will be None, Penumbral, Umbral, or Total.
If None, none of the other return values may be meaningful.

jdeMax is the jde when the center of the eclipse shadow is closest to the
Moon center, in a plane through the center of the Moon.

γ is the distance from the eclipse shadow center to the moon center
at time jdeMax.

σ is the radius of the umbral cone in the plane of the Moon.

ρ is the radius of the penumbral cone.

mag is eclipse magnitude.

sd- return values are semidurations of the phases of the eclipse, in days.

γ, σ, and ρ are in units of equatorial Earth radii.

**Kind**: static method of [<code>eclipse</code>](#module_eclipse)  
<a name="module_eclipse..snap"></a>

### eclipse~snap()
Snap returns k at specified quarter q nearest year y.
Cut and paste from moonphase.  Time corresponding to k needed in these
algorithms but otherwise not meaningful enough to export from moonphase.

**Kind**: inner method of [<code>eclipse</code>](#module_eclipse)  
<a name="module_elementequinox"></a>

## elementequinox
**License**: MIT  
**Copyright**: 2016 commenthol  

* [elementequinox](#module_elementequinox)
    * [.Elements](#module_elementequinox.Elements)
        * [new exports.Elements(inc, node, peri)](#new_module_elementequinox.Elements_new)
    * [.reduceB1950ToJ2000(eFrom)](#module_elementequinox.reduceB1950ToJ2000) ⇒ <code>Elements</code>
    * [.reduceB1950FK4ToJ2000FK5(eFrom)](#module_elementequinox.reduceB1950FK4ToJ2000FK5) ⇒ <code>Elements</code>

<a name="module_elementequinox.Elements"></a>

### elementequinox.Elements
Elements are the orbital elements of a solar system object which change
from one equinox to another.

**Kind**: static class of [<code>elementequinox</code>](#module_elementequinox)  
<a name="new_module_elementequinox.Elements_new"></a>

#### new exports.Elements(inc, node, peri)

| Param | Type | Description |
| --- | --- | --- |
| inc | <code>Number</code> | inclination |
| node | <code>Number</code> | longitude of ascending node (Ω) |
| peri | <code>Number</code> | argument of perihelion (ω) |

<a name="module_elementequinox.reduceB1950ToJ2000"></a>

### elementequinox.reduceB1950ToJ2000(eFrom) ⇒ <code>Elements</code>
ReduceB1950ToJ2000 reduces orbital elements of a solar system body from
equinox B1950 to J2000.

**Kind**: static method of [<code>elementequinox</code>](#module_elementequinox)  
**Returns**: <code>Elements</code> - eTo  

| Param | Type |
| --- | --- |
| eFrom | <code>Elements</code> | 

<a name="module_elementequinox.reduceB1950FK4ToJ2000FK5"></a>

### elementequinox.reduceB1950FK4ToJ2000FK5(eFrom) ⇒ <code>Elements</code>
ReduceB1950ToJ2000 reduces orbital elements of a solar system body from
equinox B1950 in the FK4 system to equinox J2000 in the FK5 system.

**Kind**: static method of [<code>elementequinox</code>](#module_elementequinox)  
**Returns**: <code>Elements</code> - eTo  

| Param | Type |
| --- | --- |
| eFrom | <code>Elements</code> | 

<a name="module_elliptic"></a>

## elliptic
**License**: MIT  
**Copyright**: 2016 commenthol  

* [elliptic](#module_elliptic)
    * [.Elements](#module_elliptic.Elements)
        * [.position()](#module_elliptic.Elements+position)
    * [.position()](#module_elliptic.position)
    * [.astrometricJ2000()](#module_elliptic.astrometricJ2000)
    * [.velocity()](#module_elliptic.velocity)
    * [.vAphelion()](#module_elliptic.vAphelion)
    * [.vPerihelion()](#module_elliptic.vPerihelion)
    * [.length1()](#module_elliptic.length1)
    * [.length2()](#module_elliptic.length2)
    * [.length4()](#module_elliptic.length4)

<a name="module_elliptic.Elements"></a>

### elliptic.Elements
Elements holds keplerian elements.

**Kind**: static class of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.Elements+position"></a>

#### elements.position()
Position returns observed equatorial coordinates of a body with Keplerian elements.

Argument e must be a valid V87Planet object for Earth.

Results are right ascension and declination α and δ, and elongation ψ,
all in radians.

**Kind**: instance method of [<code>Elements</code>](#module_elliptic.Elements)  
<a name="module_elliptic.position"></a>

### elliptic.position()
Position returns observed equatorial coordinates of a planet at a given time.

Argument p must be a valid V87Planet object for the observed planet.
Argument earth must be a valid V87Planet object for Earth.

Results are right ascension and declination, α and δ in radians.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.astrometricJ2000"></a>

### elliptic.astrometricJ2000()
AstrometricJ2000 is a utility function for computing astrometric coordinates.

It is used internally and only exported so that it can be used from
multiple packages.  It is not otherwise expected to be used.

Argument f is a function that returns J2000 equatorial rectangular
coodinates of a body.

Results are J2000 right ascention, declination, and elongation.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.velocity"></a>

### elliptic.velocity()
Velocity returns instantaneous velocity of a body in elliptical orbit around the Sun.

Argument a is the semimajor axis of the body, r is the instaneous distance
to the Sun, both in AU.

Result is in Km/sec.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.vAphelion"></a>

### elliptic.vAphelion()
Velocity returns the velocity of a body at aphelion.

Argument a is the semimajor axis of the body in AU, e is eccentricity.

Result is in Km/sec.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.vPerihelion"></a>

### elliptic.vPerihelion()
Velocity returns the velocity of a body at perihelion.

Argument a is the semimajor axis of the body in AU, e is eccentricity.

Result is in Km/sec.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.length1"></a>

### elliptic.length1()
Length1 returns Ramanujan's approximation for the length of an elliptical
orbit.

Argument a is semimajor axis, e is eccentricity.

Result is in units used for semimajor axis, typically AU.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.length2"></a>

### elliptic.length2()
Length2 returns an alternate approximation for the length of an elliptical
orbit.

Argument a is semimajor axis, e is eccentricity.

Result is in units used for semimajor axis, typically AU.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_elliptic.length4"></a>

### elliptic.length4()
Length4 returns the length of an elliptical orbit.

Argument a is semimajor axis, e is eccentricity.

Result is exact, and in units used for semimajor axis, typically AU.

**Kind**: static method of [<code>elliptic</code>](#module_elliptic)  
<a name="module_eqtime"></a>

## eqtime
**License**: MIT  
**Copyright**: 2016 commenthol  

* [eqtime](#module_eqtime)
    * _static_
        * [.e(jde, earth)](#module_eqtime.e) ⇒ <code>Number</code>
        * [.eSmart(jde)](#module_eqtime.eSmart) ⇒ <code>Number</code>
    * _inner_
        * [~l0()](#module_eqtime..l0)

<a name="module_eqtime.e"></a>

### eqtime.e(jde, earth) ⇒ <code>Number</code>
e computes the "equation of time" for the given JDE.

Parameter planet must be a planetposition.Planet object for Earth obtained
with `new planetposition.Planet('earth')`.

**Kind**: static method of [<code>eqtime</code>](#module_eqtime)  
**Returns**: <code>Number</code> - equation of time as an hour angle in radians.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 planet |

<a name="module_eqtime.eSmart"></a>

### eqtime.eSmart(jde) ⇒ <code>Number</code>
eSmart computes the "equation of time" for the given JDE.

Result is less accurate that e() but the function has the advantage
of not requiring the V87Planet object.

**Kind**: static method of [<code>eqtime</code>](#module_eqtime)  
**Returns**: <code>Number</code> - equation of time as an hour angle in radians.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_eqtime..l0"></a>

### eqtime~l0()
(28.2) p. 183

**Kind**: inner method of [<code>eqtime</code>](#module_eqtime)  
<a name="module_fit"></a>

## fit
**License**: MIT  
**Copyright**: 2016 commenthol  

* [fit](#module_fit)
    * [.linear()](#module_fit.linear)
    * [.correlationCoefficient()](#module_fit.correlationCoefficient)
    * [.quadratic()](#module_fit.quadratic)
    * [.func3()](#module_fit.func3)
    * [.func1()](#module_fit.func1)

<a name="module_fit.linear"></a>

### fit.linear()
Linear fits a line to sample data.

Argument p is a list of data points.  Results a and b are coefficients
of the best fit line y = ax + b.

**Kind**: static method of [<code>fit</code>](#module_fit)  
<a name="module_fit.correlationCoefficient"></a>

### fit.correlationCoefficient()
CorrelationCoefficient returns a correlation coefficient for sample data.

**Kind**: static method of [<code>fit</code>](#module_fit)  
<a name="module_fit.quadratic"></a>

### fit.quadratic()
Quadratic fits y = ax² + bx + c to sample data.

Argument p is a list of data points.  Results a, b, and c are coefficients
of the best fit quadratic y = ax² + bx + c.

**Kind**: static method of [<code>fit</code>](#module_fit)  
<a name="module_fit.func3"></a>

### fit.func3()
Func3 implements multiple linear regression for a linear combination
of three functions.

Given sample data and three functions in x, Func3 returns coefficients
a, b, and c fitting y = aƒ₀(x) + bƒ₁(x) + cƒ₂(x) to sample data.

**Kind**: static method of [<code>fit</code>](#module_fit)  
<a name="module_fit.func1"></a>

### fit.func1()
Func1 fits a linear multiple of a function to sample data.

Given sample data and a function in x, Func1 returns coefficient
a fitting y = aƒ(x).

**Kind**: static method of [<code>fit</code>](#module_fit)  
<a name="module_globe"></a>

## globe
**License**: MIT  
**Copyright**: 2016 commenthol  

* [globe](#module_globe)
    * [.Ellipsoid](#module_globe.Ellipsoid)
        * [new exports.Ellipsoid(radius, flat)](#new_module_globe.Ellipsoid_new)
        * [.A()](#module_globe.Ellipsoid+A)
        * [.B()](#module_globe.Ellipsoid+B)
        * [.eccentricity()](#module_globe.Ellipsoid+eccentricity)
        * [.parallaxConstants(φ, h)](#module_globe.Ellipsoid+parallaxConstants) ⇒ <code>Array.&lt;number&gt;</code>
        * [.rho(φ)](#module_globe.Ellipsoid+rho) ⇒ <code>number</code>
        * [.radiusAtLatitude(φ)](#module_globe.Ellipsoid+radiusAtLatitude) ⇒ <code>number</code>
        * [.radiusOfCurvature(φ)](#module_globe.Ellipsoid+radiusOfCurvature) ⇒ <code>number</code>
        * [.distance(c1, c2)](#module_globe.Ellipsoid+distance) ⇒ <code>number</code>
    * [.Coord](#module_globe.Coord)
        * [new exports.Coord(lat, lon)](#new_module_globe.Coord_new)
    * [.Earth76](#module_globe.Earth76)
    * [.RotationRate1996_5](#module_globe.RotationRate1996_5)
    * [.oneDegreeOfLongitude(rp)](#module_globe.oneDegreeOfLongitude) ⇒ <code>number</code>
    * [.oneDegreeOfLatitude(rm)](#module_globe.oneDegreeOfLatitude) ⇒ <code>number</code>
    * [.geocentricLatitudeDifference(φ)](#module_globe.geocentricLatitudeDifference) ⇒ <code>number</code>
    * [.approxAngularDistance(p1, p2)](#module_globe.approxAngularDistance) ⇒ <code>number</code>
    * [.approxLinearDistance(d)](#module_globe.approxLinearDistance) ⇒

<a name="module_globe.Ellipsoid"></a>

### globe.Ellipsoid
Ellipsoid represents an ellipsoid of revolution.

**Kind**: static class of [<code>globe</code>](#module_globe)  

* [.Ellipsoid](#module_globe.Ellipsoid)
    * [new exports.Ellipsoid(radius, flat)](#new_module_globe.Ellipsoid_new)
    * [.A()](#module_globe.Ellipsoid+A)
    * [.B()](#module_globe.Ellipsoid+B)
    * [.eccentricity()](#module_globe.Ellipsoid+eccentricity)
    * [.parallaxConstants(φ, h)](#module_globe.Ellipsoid+parallaxConstants) ⇒ <code>Array.&lt;number&gt;</code>
    * [.rho(φ)](#module_globe.Ellipsoid+rho) ⇒ <code>number</code>
    * [.radiusAtLatitude(φ)](#module_globe.Ellipsoid+radiusAtLatitude) ⇒ <code>number</code>
    * [.radiusOfCurvature(φ)](#module_globe.Ellipsoid+radiusOfCurvature) ⇒ <code>number</code>
    * [.distance(c1, c2)](#module_globe.Ellipsoid+distance) ⇒ <code>number</code>

<a name="new_module_globe.Ellipsoid_new"></a>

#### new exports.Ellipsoid(radius, flat)

| Param | Type | Description |
| --- | --- | --- |
| radius | <code>number</code> | equatorial radius |
| flat | <code>number</code> | ellipsiod flattening |

<a name="module_globe.Ellipsoid+A"></a>

#### ellipsoid.A()
A is a common identifier for equatorial radius.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
<a name="module_globe.Ellipsoid+B"></a>

#### ellipsoid.B()
B is a common identifier for polar radius.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
<a name="module_globe.Ellipsoid+eccentricity"></a>

#### ellipsoid.eccentricity()
eccentricity of a meridian.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
<a name="module_globe.Ellipsoid+parallaxConstants"></a>

#### ellipsoid.parallaxConstants(φ, h) ⇒ <code>Array.&lt;number&gt;</code>
parallaxConstants computes parallax constants ρ sin φ′ and ρ cos φ′.

Arguments are geographic latitude φ in radians and height h
in meters above the ellipsoid.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
**Returns**: <code>Array.&lt;number&gt;</code> - [ρ sin φ′, ρ cos φ] parallax constants  

| Param | Type | Description |
| --- | --- | --- |
| φ | <code>number</code> | geographic latitude in radians |
| h | <code>number</code> | height in meters above the ellipsoid |

<a name="module_globe.Ellipsoid+rho"></a>

#### ellipsoid.rho(φ) ⇒ <code>number</code>
rho is distance from Earth center to a point on the ellipsoid.

Result unit is fraction of the equatorial radius.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
**Returns**: <code>number</code> - // TODO  

| Param | Type | Description |
| --- | --- | --- |
| φ | <code>number</code> | geographic latitude in radians |

<a name="module_globe.Ellipsoid+radiusAtLatitude"></a>

#### ellipsoid.radiusAtLatitude(φ) ⇒ <code>number</code>
radiusAtLatitude returns the radius of the circle that is the parallel of
latitude at φ.

Result unit is Km.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
**Returns**: <code>number</code> - radius in km  

| Param | Type |
| --- | --- |
| φ | <code>number</code> | 

<a name="module_globe.Ellipsoid+radiusOfCurvature"></a>

#### ellipsoid.radiusOfCurvature(φ) ⇒ <code>number</code>
radiusOfCurvature of meridian at latitude φ.

Result unit is Km.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
**Returns**: <code>number</code> - radius in km  

| Param | Type |
| --- | --- |
| φ | <code>number</code> | 

<a name="module_globe.Ellipsoid+distance"></a>

#### ellipsoid.distance(c1, c2) ⇒ <code>number</code>
distance is distance between two points measured along the surface
of an ellipsoid.

Accuracy is much better than that of approxAngularDistance or
approxLinearDistance.

Result unit is Km.

**Kind**: instance method of [<code>Ellipsoid</code>](#module_globe.Ellipsoid)  
**Returns**: <code>number</code> - radius in km  

| Param | Type |
| --- | --- |
| c1 | <code>Coords</code> | 
| c2 | <code>Coords</code> | 

<a name="module_globe.Coord"></a>

### globe.Coord
Coord represents geographic coordinates on the Earth.

Longitude is measured positively westward from the Greenwich meridian.

**Kind**: static class of [<code>globe</code>](#module_globe)  
<a name="new_module_globe.Coord_new"></a>

#### new exports.Coord(lat, lon)

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| lat | <code>number</code> | <code>0</code> | latitude (φ) in radians |
| lon | <code>number</code> | <code>0</code> | longitude (ψ, or L) in radians (measured positively westward) |

<a name="module_globe.Earth76"></a>

### globe.Earth76
IAU 1976 values.  Radius in Km.

**Kind**: static constant of [<code>globe</code>](#module_globe)  
<a name="module_globe.RotationRate1996_5"></a>

### globe.RotationRate1996\_5
RotationRate1996_5 is the rotational angular velocity of the Earth
with respect to the stars at the epoch 1996.5.

Unit is radian/second.

**Kind**: static constant of [<code>globe</code>](#module_globe)  
<a name="module_globe.oneDegreeOfLongitude"></a>

### globe.oneDegreeOfLongitude(rp) ⇒ <code>number</code>
oneDegreeOfLongitude returns the length of one degree of longitude.

Argument `rp` is the radius in Km of a circle that is a parallel of latitude
(as returned by Ellipsoid.radiusAtLatitude.)
Result is distance in Km along one degree of the circle.

**Kind**: static method of [<code>globe</code>](#module_globe)  
**Returns**: <code>number</code> - distance in Km  

| Param | Type |
| --- | --- |
| rp | <code>number</code> | 

<a name="module_globe.oneDegreeOfLatitude"></a>

### globe.oneDegreeOfLatitude(rm) ⇒ <code>number</code>
oneDegreeOfLatitude returns the length of one degree of latitude.

Argument `rm` is the radius in Km of curvature along a meridian.
(as returned by Ellipsoid.radiusOfCurvature.)
Result is distance in Km along one degree of the meridian.

**Kind**: static method of [<code>globe</code>](#module_globe)  
**Returns**: <code>number</code> - distance in Km  

| Param | Type |
| --- | --- |
| rm | <code>number</code> | 

<a name="module_globe.geocentricLatitudeDifference"></a>

### globe.geocentricLatitudeDifference(φ) ⇒ <code>number</code>
geocentricLatitudeDifference returns geographic latitude - geocentric
latitude (φ - φ′) with given geographic latitude (φ).

Units are radians.

**Kind**: static method of [<code>globe</code>](#module_globe)  
**Returns**: <code>number</code> - difference in Deg  

| Param | Type |
| --- | --- |
| φ | <code>number</code> | 

<a name="module_globe.approxAngularDistance"></a>

### globe.approxAngularDistance(p1, p2) ⇒ <code>number</code>
approxAngularDistance returns the cosine of the angle between two points.

The accuracy deteriorates at small angles.

**Kind**: static method of [<code>globe</code>](#module_globe)  
**Returns**: <code>number</code> - cosine `cos` of the angle between two points.
Use `d = Math.acos(cos)` to obtain geocentric angular distance in radians  

| Param | Type | Description |
| --- | --- | --- |
| p1 | <code>Coord</code> | Point 1 |
| p2 | <code>Coord</code> | Point 2 |

<a name="module_globe.approxLinearDistance"></a>

### globe.approxLinearDistance(d) ⇒
approxLinearDistance computes a distance across the surface of the Earth.

Approximating the Earth as a sphere, the function takes a geocentric angular
distance in radians and returns the corresponding linear distance in Km.

**Kind**: static method of [<code>globe</code>](#module_globe)  
**Returns**: linear distance in Km  

| Param | Type | Description |
| --- | --- | --- |
| d | <code>number</code> | geocentric angular distance in radians |

<a name="module_illum"></a>

## illum
**License**: MIT  
**Copyright**: 2016 commenthol  

* [illum](#module_illum)
    * [.phaseAngle()](#module_illum.phaseAngle)
    * [.fraction()](#module_illum.fraction)
    * [.phaseAngle2()](#module_illum.phaseAngle2)
    * [.phaseAngle3()](#module_illum.phaseAngle3)
    * [.fractionVenus()](#module_illum.fractionVenus)
    * [.mercury()](#module_illum.mercury)
    * [.venus()](#module_illum.venus)
    * [.mars()](#module_illum.mars)
    * [.jupiter()](#module_illum.jupiter)
    * [.saturn()](#module_illum.saturn)
    * [.uranus()](#module_illum.uranus)
    * [.neptune()](#module_illum.neptune)
    * [.mercury84()](#module_illum.mercury84)
    * [.venus84()](#module_illum.venus84)
    * [.mars84()](#module_illum.mars84)
    * [.jupiter84()](#module_illum.jupiter84)
    * [.saturn84()](#module_illum.saturn84)
    * [.uranus84()](#module_illum.uranus84)
    * [.neptune84()](#module_illum.neptune84)
    * [.pluto84()](#module_illum.pluto84)

<a name="module_illum.phaseAngle"></a>

### illum.phaseAngle()
PhaseAngle computes the phase angle of a planet.

Argument r is planet's distance to Sun, Δ its distance to Earth, and R
the distance from Sun to Earth.  All distances in AU.

Result in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.fraction"></a>

### illum.fraction()
Fraction computes the illuminated fraction of the disk of a planet.

Argument r is planet's distance to Sun, Δ its distance to Earth, and R
the distance from Sun to Earth.  All distances in AU.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.phaseAngle2"></a>

### illum.phaseAngle2()
PhaseAngle2 computes the phase angle of a planet.

Arguments L, B, R are heliocentric ecliptical coordinates of the planet.
L0, R0 are longitude and radius for Earth, Δ is distance from Earth to
the planet.  All distances in AU, angles in radians.

The phase angle result is in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.phaseAngle3"></a>

### illum.phaseAngle3()
PhaseAngle3 computes the phase angle of a planet.

Arguments L, B are heliocentric ecliptical longitude and latitude of the
planet.  x, y, z are cartesian coordinates of the planet, Δ is distance
from Earth to the planet.  All distances in AU, angles in radians.

The phase angle result is in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.fractionVenus"></a>

### illum.fractionVenus()
FractionVenus computes an approximation of the illumanted fraction of Venus.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.mercury"></a>

### illum.mercury()
Mercury computes the visual magnitude of Mercury.
Formula by G. Müller

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.venus"></a>

### illum.venus()
Venus computes the visual magnitude of Venus.
Formula by G. Müller

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.mars"></a>

### illum.mars()
Mars computes the visual magnitude of Mars.
Formula by G. Müller

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.jupiter"></a>

### illum.jupiter()
Jupiter computes the visual magnitude of Jupiter.
Formula by G. Müller
Effect of phase not considered

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.saturn"></a>

### illum.saturn()
Saturn computes the visual magnitude of Saturn.
Formula by G. Müller
Sun's altitude above the plane of the ring is not considered.

Argument r is the planet's distance from the Sun, Δ the distance from Earth.
B is the Saturnicentric latitude of the Earth referred to the plane of
Saturn's ring.
ΔU (in radians) is the difference between the Saturnicentric longitudes
of the Sun and the Earth, measured in the plane of the ring.
You can use saturndisk.Disk() to obtain B and ΔU.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.uranus"></a>

### illum.uranus()
Uranus computes the visual magnitude of Uranus.
Formula by G. Müller

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.neptune"></a>

### illum.neptune()
Neptune computes the visual magnitude of Neptune.
Formulae by G. Müller

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.mercury84"></a>

### illum.mercury84()
Mercury84 computes the visual magnitude of Mercury.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.venus84"></a>

### illum.venus84()
Venus84 computes the visual magnitude of Venus.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.mars84"></a>

### illum.mars84()
Mars84 computes the visual magnitude of Mars.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.jupiter84"></a>

### illum.jupiter84()
Jupiter84 computes the visual magnitude of Jupiter.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth,
and i the phase angle in radians.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.saturn84"></a>

### illum.saturn84()
Saturn84 computes the visual magnitude of Saturn.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth.
B is the Saturnicentric latitude of the Earth referred to the plane of
Saturn's ring.
ΔU (in radians) is the difference between the Saturnicentric longitudes
of the Sun and the Earth, measured in the plane of the ring.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.uranus84"></a>

### illum.uranus84()
Uranus84 computes the visual magnitude of Uranus.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.neptune84"></a>

### illum.neptune84()
Neptune84 computes the visual magnitude of Neptune.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_illum.pluto84"></a>

### illum.pluto84()
Pluto84 computes the visual magnitude of Pluto.
The formula is that adopted in "Astronomical Almanac" in 1984.0

Argument r is the planet's distance from the Sun, Δ the distance from Earth.

**Kind**: static method of [<code>illum</code>](#module_illum)  
<a name="module_interpolation"></a>

## interpolation
**License**: MIT  
**Copyright**: 2016 commenthol  

* [interpolation](#module_interpolation)
    * [.Len3](#module_interpolation.Len3)
        * [new exports.Len3(x1, x3, y)](#new_module_interpolation.Len3_new)
        * [.interpolateX()](#module_interpolation.Len3+interpolateX)
        * [.interpolateXStrict()](#module_interpolation.Len3+interpolateXStrict)
        * [.interpolateN()](#module_interpolation.Len3+interpolateN)
        * [.interpolateNStrict()](#module_interpolation.Len3+interpolateNStrict)
        * [.extremum()](#module_interpolation.Len3+extremum)
        * [.zero()](#module_interpolation.Len3+zero)
    * [.Len5](#module_interpolation.Len5)
        * [new exports.Len5()](#new_module_interpolation.Len5_new)
        * [.interpolateX()](#module_interpolation.Len5+interpolateX)
        * [.interpolateXStrict()](#module_interpolation.Len5+interpolateXStrict)
        * [.interpolateN()](#module_interpolation.Len5+interpolateN)
        * [.interpolateNStrict()](#module_interpolation.Len5+interpolateNStrict)
        * [.extremum()](#module_interpolation.Len5+extremum)
        * [.zero()](#module_interpolation.Len5+zero)
    * [.errorNot3](#module_interpolation.errorNot3)
    * [.len3ForInterpolateX(x, x1, xn, y)](#module_interpolation.len3ForInterpolateX) ⇒ <code>Number</code>
    * [.len4Half(y)](#module_interpolation.len4Half) ⇒ <code>Number</code>
    * [.lagrange(x, table)](#module_interpolation.lagrange) ⇒ <code>Number</code>
    * [.lagrangePoly(table)](#module_interpolation.lagrangePoly) ⇒ <code>Array</code>
    * [.linear()](#module_interpolation.linear)

<a name="module_interpolation.Len3"></a>

### interpolation.Len3
Len3 allows second difference interpolation.

**Kind**: static class of [<code>interpolation</code>](#module_interpolation)  

* [.Len3](#module_interpolation.Len3)
    * [new exports.Len3(x1, x3, y)](#new_module_interpolation.Len3_new)
    * [.interpolateX()](#module_interpolation.Len3+interpolateX)
    * [.interpolateXStrict()](#module_interpolation.Len3+interpolateXStrict)
    * [.interpolateN()](#module_interpolation.Len3+interpolateN)
    * [.interpolateNStrict()](#module_interpolation.Len3+interpolateNStrict)
    * [.extremum()](#module_interpolation.Len3+extremum)
    * [.zero()](#module_interpolation.Len3+zero)

<a name="new_module_interpolation.Len3_new"></a>

#### new exports.Len3(x1, x3, y)
NewLen3 prepares a Len3 object from a table of three rows of x and y values.

X values must be equally spaced, so only the first and last are supplied.
X1 must not equal to x3.  Y must be a slice of three y values.

**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| x1 | <code>Number</code> | is the x value corresponding to the first y value of the table. |
| x3 | <code>Number</code> | is the x value corresponding to the last y value of the table. |
| y | <code>Array.&lt;Number&gt;</code> | is all y values in the table. y.length should be >= 3.0 |

<a name="module_interpolation.Len3+interpolateX"></a>

#### len3.interpolateX()
InterpolateX interpolates for a given x value.

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len3+interpolateXStrict"></a>

#### len3.interpolateXStrict()
InterpolateXStrict interpolates for a given x value,
restricting x to the range x1 to x3 given to the constructor NewLen3.

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len3+interpolateN"></a>

#### len3.interpolateN()
InterpolateN interpolates for (a given interpolating factor n.

This is interpolation formula (3.3)

The interpolation factor n is x-x2 in units of the tabular x interval.
(See Meeus p. 24.)

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len3+interpolateNStrict"></a>

#### len3.interpolateNStrict()
InterpolateNStrict interpolates for (a given interpolating factor n.

N is restricted to the range [-1..1] corresponding to the range x1 to x3
given to the constructor of Len3.

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len3+extremum"></a>

#### len3.extremum()
Extremum returns the x and y values at the extremum.

Results are restricted to the range of the table given to the constructor
new Len3.

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len3+zero"></a>

#### len3.zero()
Len3Zero finds a zero of the quadratic function represented by the table.

That is, it returns an x value that yields y=0.

Argument strong switches between two strategies for the estimation step.
when iterating to converge on the zero.

Strong=false specifies a quick and dirty estimate that works well
for gentle curves, but can work poorly or fail on more dramatic curves.

Strong=true specifies a more sophisticated and thus somewhat more
expensive estimate.  However, if the curve has quick changes, This estimate
will converge more reliably and in fewer steps, making it a better choice.

Results are restricted to the range of the table given to the constructor
NewLen3.

**Kind**: instance method of [<code>Len3</code>](#module_interpolation.Len3)  
<a name="module_interpolation.Len5"></a>

### interpolation.Len5
Len5 allows fourth Difference interpolation.

**Kind**: static class of [<code>interpolation</code>](#module_interpolation)  

* [.Len5](#module_interpolation.Len5)
    * [new exports.Len5()](#new_module_interpolation.Len5_new)
    * [.interpolateX()](#module_interpolation.Len5+interpolateX)
    * [.interpolateXStrict()](#module_interpolation.Len5+interpolateXStrict)
    * [.interpolateN()](#module_interpolation.Len5+interpolateN)
    * [.interpolateNStrict()](#module_interpolation.Len5+interpolateNStrict)
    * [.extremum()](#module_interpolation.Len5+extremum)
    * [.zero()](#module_interpolation.Len5+zero)

<a name="new_module_interpolation.Len5_new"></a>

#### new exports.Len5()
NewLen5 prepares a Len5 object from a table of five rows of x and y values.

X values must be equally spaced, so only the first and last are suppliethis.
X1 must not equal x5.  Y must be a slice of five y values.

<a name="module_interpolation.Len5+interpolateX"></a>

#### len5.interpolateX()
InterpolateX interpolates for (a given x value.

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.Len5+interpolateXStrict"></a>

#### len5.interpolateXStrict()
InterpolateXStrict interpolates for a given x value,
restricting x to the range x1 to x5 given to the the constructor NewLen5.

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.Len5+interpolateN"></a>

#### len5.interpolateN()
InterpolateN interpolates for (a given interpolating factor n.

The interpolation factor n is x-x3 in units of the tabular x interval.
(See Meeus p. 28.)

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.Len5+interpolateNStrict"></a>

#### len5.interpolateNStrict()
InterpolateNStrict interpolates for (a given interpolating factor n.

N is restricted to the range [-1..1].  This is only half the range given
to the constructor NewLen5, but is the recommendation given on p. 31.0

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.Len5+extremum"></a>

#### len5.extremum()
Extremum returns the x and y values at the extremum.

Results are restricted to the range of the table given to the constructor
NewLen5.  (Meeus actually recommends restricting the range to one unit of
the tabular interval, but that seems a little harsh.)

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.Len5+zero"></a>

#### len5.zero()
Len5Zero finds a zero of the quartic function represented by the table.

That is, it returns an x value that yields y=0.

Argument strong switches between two strategies for the estimation step.
when iterating to converge on the zero.

Strong=false specifies a quick and dirty estimate that works well
for gentle curves, but can work poorly or fail on more dramatic curves.

Strong=true specifies a more sophisticated and thus somewhat more
expensive estimate.  However, if the curve has quick changes, This estimate
will converge more reliably and in fewer steps, making it a better choice.

Results are restricted to the range of the table given to the constructor
NewLen5.

**Kind**: instance method of [<code>Len5</code>](#module_interpolation.Len5)  
<a name="module_interpolation.errorNot3"></a>

### interpolation.errorNot3
Error values returned by functions and methods in this package.
Defined here to help testing for specific errors.

**Kind**: static constant of [<code>interpolation</code>](#module_interpolation)  
<a name="module_interpolation.len3ForInterpolateX"></a>

### interpolation.len3ForInterpolateX(x, x1, xn, y) ⇒ <code>Number</code>
Len3ForInterpolateX is a special purpose Len3 constructor.

Like NewLen3, it takes a table of x and y values, but it is not limited
to tables of 3 rows.  An X value is also passed that represents the
interpolation target x value.  Len3ForInterpolateX will locate the
appropriate three rows of the table for interpolating for x, and initialize
the Len3 object for those rows.

**Kind**: static method of [<code>interpolation</code>](#module_interpolation)  
**Returns**: <code>Number</code> - interpolation value  

| Param | Type | Description |
| --- | --- | --- |
| x | <code>Number</code> | is the target for interpolation |
| x1 | <code>Number</code> | is the x value corresponding to the first y value of the table. |
| xn | <code>Number</code> | is the x value corresponding to the last y value of the table. |
| y | <code>Array.&lt;Number&gt;</code> | is all y values in the table.  y.length should be >= 3.0 |

<a name="module_interpolation.len4Half"></a>

### interpolation.len4Half(y) ⇒ <code>Number</code>
Len4Half interpolates a center value from a table of four rows.

**Kind**: static method of [<code>interpolation</code>](#module_interpolation)  
**Returns**: <code>Number</code> - interpolation result  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Array.&lt;Number&gt;</code> | 4 values |

<a name="module_interpolation.lagrange"></a>

### interpolation.lagrange(x, table) ⇒ <code>Number</code>
Lagrange performs interpolation with unequally-spaced abscissae.

Given a table of X and Y values, interpolate a new y value for argument x.

X values in the table do not have to be equally spaced; they do not even
have to be in order. They must however, be distinct.

**Kind**: static method of [<code>interpolation</code>](#module_interpolation)  
**Returns**: <code>Number</code> - interpolation result `y` of `x`  

| Param | Type | Description |
| --- | --- | --- |
| x | <code>Number</code> | x-value of interpolation |
| table | <code>Array</code> | `[[x0, y0], ... [xN, yN]]` of x, y values |

<a name="module_interpolation.lagrangePoly"></a>

### interpolation.lagrangePoly(table) ⇒ <code>Array</code>
LagrangePoly uses the formula of Lagrange to produce an interpolating
polynomial.

X values in the table do not have to be equally spaced; they do not even
have to be in order.  They must however, be distinct.

The returned polynomial will be of degree n-1 where n is the number of rows
in the table.  It can be evaluated for x using base.horner.

**Kind**: static method of [<code>interpolation</code>](#module_interpolation)  
**Returns**: <code>Array</code> - - polynomial array  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>Array</code> | `[[x0, y0], ... [xN, yN]]` |

<a name="module_interpolation.linear"></a>

### interpolation.linear()
Linear Interpolation of x

**Kind**: static method of [<code>interpolation</code>](#module_interpolation)  
<a name="module_iterate"></a>

## iterate
**License**: MIT  
**Copyright**: 2016 commenthol  

* [iterate](#module_iterate)
    * [.decimalPlaces(better, start, places, maxIterations)](#module_iterate.decimalPlaces) ⇒ <code>Number</code>
    * [.fullPrecision(better, start, maxIterations)](#module_iterate.fullPrecision) ⇒ <code>Number</code>
    * [.binaryRoot(f, lower, upper)](#module_iterate.binaryRoot) ⇒ <code>Number</code>

<a name="module_iterate.decimalPlaces"></a>

### iterate.decimalPlaces(better, start, places, maxIterations) ⇒ <code>Number</code>
decimalPlaces iterates to a fixed number of decimal places.

Inputs are an improvement function, a starting value, the number of
decimal places desired in the result, and an iteration limit.

**Kind**: static method of [<code>iterate</code>](#module_iterate)  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| better | <code>function</code> |  |
| start | <code>Number</code> | (float) |
| places | <code>Number</code> | (int) |
| maxIterations | <code>Number</code> | (int) |

<a name="module_iterate.fullPrecision"></a>

### iterate.fullPrecision(better, start, maxIterations) ⇒ <code>Number</code>
fullPrecison iterates to (nearly) the full precision of a float64.

To allow for a little bit of floating point jitter, FullPrecision iterates
to 15 significant figures, which is the maximum number of full significant
figures representable in a float64, but still a couple of bits shy of the
full representable precision.

**Kind**: static method of [<code>iterate</code>](#module_iterate)  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| better | <code>function</code> |  |
| start | <code>Number</code> | (float) |
| maxIterations | <code>Number</code> | (int) |

<a name="module_iterate.binaryRoot"></a>

### iterate.binaryRoot(f, lower, upper) ⇒ <code>Number</code>
binaryRoot finds a root between given bounds by binary search.

Inputs are a function on x and the bounds on x.  A root must exist between
the given bounds, otherwise the result is not meaningful.

**Kind**: static method of [<code>iterate</code>](#module_iterate)  

| Param | Type | Description |
| --- | --- | --- |
| f | <code>function</code> | root function |
| lower | <code>Number</code> | (float) |
| upper | <code>Number</code> | (float) |

<a name="module_jm"></a>

## jm
**License**: MIT  
**Copyright**: 2016 commenthol  

* [jm](#module_jm)
    * _static_
        * [.JewishCalendar()](#module_jm.JewishCalendar)
        * [.MoslemToJD(y, m, d)](#module_jm.MoslemToJD) ⇒ <code>Number</code>
        * [.MoslemLeapYear(year)](#module_jm.MoslemLeapYear) ⇒ <code>Boolean</code>
        * [.JulianToMoslem(y, m, d)](#module_jm.JulianToMoslem) ⇒ <code>Array</code>
        * [.moslemMonth()](#module_jm.moslemMonth)
    * _inner_
        * [~mmonths](#module_jm..mmonths)

<a name="module_jm.JewishCalendar"></a>

### jm.JewishCalendar()
JewishCalendar returns interesting dates and facts about a given year.

Input is a Julian or Gregorian year.

Outputs:
 A:      (int) Year number in the Jewish Calendar
 mP:     (int) Month number of Pesach.
 dP:     (int) Day number of Pesach.
 mNY:    (int) Month number of the Jewish new year.
 dNY:    (int) Day number of the Jewish new year.
 months: (int) Number of months in this year.
 days:   (int) Number of days in this year.

**Kind**: static method of [<code>jm</code>](#module_jm)  
<a name="module_jm.MoslemToJD"></a>

### jm.MoslemToJD(y, m, d) ⇒ <code>Number</code>
MoslemToJD converts a Moslem calendar date to a Julian Day.

**Kind**: static method of [<code>jm</code>](#module_jm)  
**Returns**: <code>Number</code> - jd - Julian day  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | year in moslem calendar |
| m | <code>Number</code> | month |
| d | <code>Number</code> | day |

<a name="module_jm.MoslemLeapYear"></a>

### jm.MoslemLeapYear(year) ⇒ <code>Boolean</code>
MoslemLeapYear returns true if year y of the Moslem calendar is a leap year.

**Kind**: static method of [<code>jm</code>](#module_jm)  
**Returns**: <code>Boolean</code> - true if leap year  

| Param | Type |
| --- | --- |
| year | <code>Number</code> | 

<a name="module_jm.JulianToMoslem"></a>

### jm.JulianToMoslem(y, m, d) ⇒ <code>Array</code>
JulianToMoslem takes a year, month, and day of the Julian calendar and returns the equivalent year, month, and day of the Moslem calendar.

**Kind**: static method of [<code>jm</code>](#module_jm)  
**Returns**: <code>Array</code> - [my, mm, md]  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | julian year |
| m | <code>Number</code> | julian month |
| d | <code>Number</code> | julian day |

<a name="module_jm.moslemMonth"></a>

### jm.moslemMonth()
String returns the Romanization of the month ("Muḥarram", "Ṣafar", ...).

**Kind**: static method of [<code>jm</code>](#module_jm)  
<a name="module_jm..mmonths"></a>

### jm~mmonths
An MMonth specifies a month of the Moslum Calendar (Muharram = 1, ...).

Upgraded to Unicode from the spellings given by Meeus.
Source: http://en.wikipedia.org/wiki/Islamic_calendar.

**Kind**: inner constant of [<code>jm</code>](#module_jm)  
<a name="module_julian"></a>

## julian
**License**: MIT  
**Copyright**: 2016 commenthol  

* [julian](#module_julian)
    * [.Calendar](#module_julian.Calendar)
        * [new exports.Calendar(year, month, day)](#new_module_julian.Calendar_new)
        * [.fromDate(date)](#module_julian.Calendar+fromDate)
        * [.toDate()](#module_julian.Calendar+toDate) ⇒ <code>Date</code>
        * [.toYear()](#module_julian.Calendar+toYear) ⇒ <code>number</code>
        * [.fromYear(decimal)](#module_julian.Calendar+fromYear)
        * [.midnight()](#module_julian.Calendar+midnight)
        * [.noon()](#module_julian.Calendar+noon)
        * [.deltaT(td)](#module_julian.Calendar+deltaT)
    * [.GREGORIAN0JD](#module_julian.GREGORIAN0JD)
    * [.CalendarToJD()](#module_julian.CalendarToJD)
    * [.CalendarGregorianToJD(y, m, d)](#module_julian.CalendarGregorianToJD) ⇒ <code>number</code>
    * [.CalendarJulianToJD(y, m, d)](#module_julian.CalendarJulianToJD) ⇒ <code>number</code>
    * [.LeapYearJulian(y)](#module_julian.LeapYearJulian) ⇒ <code>boolean</code>
    * [.LeapYearGregorian(y)](#module_julian.LeapYearGregorian) ⇒ <code>boolean</code>
    * [.JDToCalendar(jd, isJulian)](#module_julian.JDToCalendar) ⇒ <code>object</code>
    * [.JDToCalendarGregorian(jd)](#module_julian.JDToCalendarGregorian) ⇒ <code>object</code>
    * [.JDToCalendarJulian(jd)](#module_julian.JDToCalendarJulian) ⇒ <code>object</code>
    * [.isJDCalendarGregorian(jd)](#module_julian.isJDCalendarGregorian) ⇒ <code>boolean</code>
    * [.isCalendarGregorian(year, [month], [day])](#module_julian.isCalendarGregorian) ⇒ <code>boolean</code>
    * [.JDToDate(jd)](#module_julian.JDToDate) ⇒ <code>Date</code>
    * [.DateToJD(date)](#module_julian.DateToJD) ⇒ <code>number</code>
    * [.JDEToDate(jde)](#module_julian.JDEToDate) ⇒ <code>Date</code>
    * [.DateToJDE(date)](#module_julian.DateToJDE) ⇒ <code>number</code>
    * [.MJDToJD(mjd)](#module_julian.MJDToJD) ⇒ <code>Number</code>
    * [.JDToMJD(jd)](#module_julian.JDToMJD) ⇒ <code>Number</code>
    * [.DayOfWeek(jd)](#module_julian.DayOfWeek) ⇒ <code>number</code>
    * [.DayOfYearGregorian(y, m, d)](#module_julian.DayOfYearGregorian) ⇒ <code>number</code>
    * [.DayOfYearJulian(y, m, d)](#module_julian.DayOfYearJulian) ⇒ <code>number</code>
    * [.DayOfYear(y, m, d, leap)](#module_julian.DayOfYear) ⇒ <code>number</code>
    * [.DayOfYearToCalendar(n, leap)](#module_julian.DayOfYearToCalendar) ⇒ <code>object</code>
    * [.DayOfYearToCalendarGregorian(year, n)](#module_julian.DayOfYearToCalendarGregorian) ⇒ <code>CalendarGregorian</code>
    * [.DayOfYearToCalendarJulian(year, n)](#module_julian.DayOfYearToCalendarJulian) ⇒ <code>CalendarJulian</code>

<a name="module_julian.Calendar"></a>

### julian.Calendar
Base class for CalendarJulian and CalendarGregorian
Respects the start of the Gregorian Calendar at `GREGORIAN0JD`

**Kind**: static class of [<code>julian</code>](#module_julian)  

* [.Calendar](#module_julian.Calendar)
    * [new exports.Calendar(year, month, day)](#new_module_julian.Calendar_new)
    * [.fromDate(date)](#module_julian.Calendar+fromDate)
    * [.toDate()](#module_julian.Calendar+toDate) ⇒ <code>Date</code>
    * [.toYear()](#module_julian.Calendar+toYear) ⇒ <code>number</code>
    * [.fromYear(decimal)](#module_julian.Calendar+fromYear)
    * [.midnight()](#module_julian.Calendar+midnight)
    * [.noon()](#module_julian.Calendar+noon)
    * [.deltaT(td)](#module_julian.Calendar+deltaT)

<a name="new_module_julian.Calendar_new"></a>

#### new exports.Calendar(year, month, day)

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| year | <code>number</code> \| <code>Date</code> |  | If `Date` is given then year, month, day is taken from that. Shortcut to `new Calendar().fromDate(date)` |
| month | <code>number</code> | <code>1</code> |  |
| day | <code>number</code> | <code>1</code> |  |

<a name="module_julian.Calendar+fromDate"></a>

#### calendar.fromDate(date)
Note: Take care for dates < GREGORIAN0JD as `date` is always within the
proleptic Gregorian Calender

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  

| Param | Type | Description |
| --- | --- | --- |
| date | <code>Date</code> | proleptic Gregorian date |

<a name="module_julian.Calendar+toDate"></a>

#### calendar.toDate() ⇒ <code>Date</code>
Note: Take care for dates < GREGORIAN0JD as `date` is always within the
proleptic Gregorian Calender

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  
**Returns**: <code>Date</code> - proleptic Gregorian date  
<a name="module_julian.Calendar+toYear"></a>

#### calendar.toYear() ⇒ <code>number</code>
converts a calendar date to decimal year

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  
**Returns**: <code>number</code> - decimal year  
<a name="module_julian.Calendar+fromYear"></a>

#### calendar.fromYear(decimal)
converts a decimal year to a calendar date

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  

| Param | Type | Description |
| --- | --- | --- |
| decimal | <code>number</code> | year |

<a name="module_julian.Calendar+midnight"></a>

#### calendar.midnight()
set date to midnight UTC

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  
<a name="module_julian.Calendar+noon"></a>

#### calendar.noon()
set date to noon UTC

**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  
<a name="module_julian.Calendar+deltaT"></a>

#### calendar.deltaT(td)
**Kind**: instance method of [<code>Calendar</code>](#module_julian.Calendar)  

| Param | Type | Description |
| --- | --- | --- |
| td | <code>Boolean</code> | if `true` calendar instance is in TD; date gets converted to UT   true  - `UT = TD - ΔT`   false - `TD = UT + ΔT` |

<a name="module_julian.GREGORIAN0JD"></a>

### julian.GREGORIAN0JD
1582-10-05 Julian Date is 1st Gregorian Date (1582-10-15)

**Kind**: static constant of [<code>julian</code>](#module_julian)  
<a name="module_julian.CalendarToJD"></a>

### julian.CalendarToJD()
base conversion from calendar date to julian day

**Kind**: static method of [<code>julian</code>](#module_julian)  
<a name="module_julian.CalendarGregorianToJD"></a>

### julian.CalendarGregorianToJD(y, m, d) ⇒ <code>number</code>
CalendarGregorianToJD converts a Gregorian year, month, and day of month
to Julian day.

Negative years are valid, back to JD 0.  The result is not valid for
dates before JD 0.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - jd - Julian day (float)  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |
| m | <code>number</code> | month (int) |
| d | <code>number</code> | day (float) |

<a name="module_julian.CalendarJulianToJD"></a>

### julian.CalendarJulianToJD(y, m, d) ⇒ <code>number</code>
CalendarJulianToJD converts a Julian year, month, and day of month to Julian day.

Negative years are valid, back to JD 0.  The result is not valid for
dates before JD 0.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - jd - Julian day (float)  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |
| m | <code>number</code> | month (int) |
| d | <code>number</code> | day (float) |

<a name="module_julian.LeapYearJulian"></a>

### julian.LeapYearJulian(y) ⇒ <code>boolean</code>
LeapYearJulian returns true if year y in the Julian calendar is a leap year.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>boolean</code> - true if leap year in Julian Calendar  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |

<a name="module_julian.LeapYearGregorian"></a>

### julian.LeapYearGregorian(y) ⇒ <code>boolean</code>
LeapYearGregorian returns true if year y in the Gregorian calendar is a leap year.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>boolean</code> - true if leap year in Gregorian Calendar  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |

<a name="module_julian.JDToCalendar"></a>

### julian.JDToCalendar(jd, isJulian) ⇒ <code>object</code>
JDToCalendar returns the calendar date for the given jd.

Note that this function returns a date in either the Julian or Gregorian
Calendar, as appropriate.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>object</code> - `{ (int) year, (int) month, (float) day }`  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |
| isJulian | <code>boolean</code> | set true for Julian Calendar, otherwise Gregorian is used |

<a name="module_julian.JDToCalendarGregorian"></a>

### julian.JDToCalendarGregorian(jd) ⇒ <code>object</code>
JDToCalendarGregorian returns the calendar date for the given jd in the Gregorian Calendar.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>object</code> - `{ (int) year, (int) month, (float) day }`  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |

<a name="module_julian.JDToCalendarJulian"></a>

### julian.JDToCalendarJulian(jd) ⇒ <code>object</code>
JDToCalendarJulian returns the calendar date for the given jd in the Julian Calendar.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>object</code> - { (int) year, (int) month, (float) day }  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |

<a name="module_julian.isJDCalendarGregorian"></a>

### julian.isJDCalendarGregorian(jd) ⇒ <code>boolean</code>
isJDCalendarGregorian tests if Julian day `jd` falls into the Gregorian calendar

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>boolean</code> - true for Gregorian, false for Julian calendar  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |

<a name="module_julian.isCalendarGregorian"></a>

### julian.isCalendarGregorian(year, [month], [day]) ⇒ <code>boolean</code>
isCalendarGregorian tests if date falls into the Gregorian calendar

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>boolean</code> - true for Gregorian, false for Julian calendar  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>number</code> | julian/gregorian year |
| [month] | <code>number</code> | month of julian/gregorian year |
| [day] | <code>number</code> | day of julian/gregorian year |

<a name="module_julian.JDToDate"></a>

### julian.JDToDate(jd) ⇒ <code>Date</code>
JDToDate converts a Julian day `jd` to a Date Object (Gregorian Calendar)

Note: Javascript uses the the ISO-8601 calendar, which is a proleptic Gregorian
calendar, i.e. it acts as if this calendar was always in effect, even before
its year of introduction in 1582. Therefore dates between 1582-10-05 and
1582-10-14 exists.

**Kind**: static method of [<code>julian</code>](#module_julian)  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |

<a name="module_julian.DateToJD"></a>

### julian.DateToJD(date) ⇒ <code>number</code>
DateToJD converts a proleptic Gregorian Date into a Julian day `jd`

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - jd - Julian day (float)  

| Param | Type |
| --- | --- |
| date | <code>Date</code> | 

<a name="module_julian.JDEToDate"></a>

### julian.JDEToDate(jde) ⇒ <code>Date</code>
JDEToDate converts a Julian ephemeris day `jde` to a Date Object (Gregorian Calendar)
To obtain "Universal Time" (UT) from "Dynamical Time" (TD) the correction ΔT (in seconds) gets applied
```
UT = TD - ΔT
```
If your use case does not require such accuracy converting `jde` using `JDToDate` is fine.

Note: Javascript uses the the ISO-8601 calendar, which is a proleptic Gregorian
calendar, i.e. it acts as if this calendar was always in effect, even before
its year of introduction in 1582. Therefore dates between 1582-10-05 and
1582-10-14 exists.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>Date</code> - Javascript Date Object  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_julian.DateToJDE"></a>

### julian.DateToJDE(date) ⇒ <code>number</code>
DateToJDE converts a Date Object (Gregorian Calendar) to a Julian ephemeris day `jde`
To obtain "Dynamical Time" (TD) from "Universal Time" (UT) the correction ΔT (in seconds) gets applied
```
TD = UT + ΔT
```
If your use case does not require such accuracy converting `Date` using `DateToJD` is fine.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - jde - Julian ephemeris day (float)  

| Param | Type | Description |
| --- | --- | --- |
| date | <code>Date</code> | Javascript Date Object |

<a name="module_julian.MJDToJD"></a>

### julian.MJDToJD(mjd) ⇒ <code>Number</code>
converts Modified Julian Day `mjd` to Julian Day `jd`

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>Number</code> - jd - Julian Day  

| Param | Type | Description |
| --- | --- | --- |
| mjd | <code>Number</code> | Modified Julian Day |

<a name="module_julian.JDToMJD"></a>

### julian.JDToMJD(jd) ⇒ <code>Number</code>
converts Julian Day `jd` to Modified Julian Day `mjd`

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>Number</code> - mjd - Modified Julian Day  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>Number</code> | Julian Day |

<a name="module_julian.DayOfWeek"></a>

### julian.DayOfWeek(jd) ⇒ <code>number</code>
DayOfWeek determines the day of the week for a given JD.

The value returned is an integer in the range 0 to 6, where 0 represents
Sunday.  This is the same convention followed in the time package of the
Javascript standard library.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - (int) 0 == sunday; ...; 6 == saturday  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian day (float) |

<a name="module_julian.DayOfYearGregorian"></a>

### julian.DayOfYearGregorian(y, m, d) ⇒ <code>number</code>
DayOfYearGregorian computes the day number within the year of the Gregorian
calendar.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - day of year  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |
| m | <code>number</code> | month (int) |
| d | <code>number</code> | day (float) |

<a name="module_julian.DayOfYearJulian"></a>

### julian.DayOfYearJulian(y, m, d) ⇒ <code>number</code>
DayOfYearJulian computes the day number within the year of the Julian
calendar.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - day of year  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |
| m | <code>number</code> | month (int) |
| d | <code>number</code> | day (float) |

<a name="module_julian.DayOfYear"></a>

### julian.DayOfYear(y, m, d, leap) ⇒ <code>number</code>
DayOfYear computes the day number within the year.

This form of the function is not specific to the Julian or Gregorian
calendar, but you must tell it whether the year is a leap year.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>number</code> - day of year  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>number</code> | year (int) |
| m | <code>number</code> | month (int) |
| d | <code>number</code> | day (float) |
| leap | <code>boolean</code> | set `true` if `y` is leap year |

<a name="module_julian.DayOfYearToCalendar"></a>

### julian.DayOfYearToCalendar(n, leap) ⇒ <code>object</code>
DayOfYearToCalendar returns the calendar month and day for a given
day of year and leap year status.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>object</code> - `{ (int) month, (float) day }`  

| Param | Type | Description |
| --- | --- | --- |
| n | <code>number</code> | day of year (int) |
| leap | <code>boolean</code> | set `true` if `y` is leap year |

<a name="module_julian.DayOfYearToCalendarGregorian"></a>

### julian.DayOfYearToCalendarGregorian(year, n) ⇒ <code>CalendarGregorian</code>
DayOfYearToCalendarGregorian returns the calendar month and day for a given
day of year.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>CalendarGregorian</code> - { (int) year, (int) month, (float) day }  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>number</code> |  |
| n | <code>number</code> | day of year (int) |

<a name="module_julian.DayOfYearToCalendarJulian"></a>

### julian.DayOfYearToCalendarJulian(year, n) ⇒ <code>CalendarJulian</code>
DayOfYearToCalendarJulian returns the calendar month and day for a given
day of year.

**Kind**: static method of [<code>julian</code>](#module_julian)  
**Returns**: <code>CalendarJulian</code> - { (int) year, (int) month, (float) day }  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>number</code> |  |
| n | <code>number</code> | day of year (int) |

<a name="module_jupiter"></a>

## jupiter
**License**: MIT  
**Copyright**: 2016 commenthol  

* [jupiter](#module_jupiter)
    * [.physical(jde, earth, jupiter)](#module_jupiter.physical) ⇒ <code>Array</code>
    * [.physical2(jde)](#module_jupiter.physical2) ⇒ <code>Array</code>

<a name="module_jupiter.physical"></a>

### jupiter.physical(jde, earth, jupiter) ⇒ <code>Array</code>
Physical computes quantities for physical observations of Jupiter.

All angular results in radians.

**Kind**: static method of [<code>jupiter</code>](#module_jupiter)  
**Returns**: <code>Array</code> - {number} DS - Planetocentric declination of the Sun.
   {number} DE - Planetocentric declination of the Earth.
   {number} ω1 - Longitude of the System I central meridian of the illuminated disk,
                 as seen from Earth.
   {number} ω2 - Longitude of the System II central meridian of the illuminated disk,
                 as seen from Earth.
   {number} P -  Geocentric position angle of Jupiter's northern rotation pole.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> |  |
| jupiter | <code>planetposition.Planet</code> |  |

<a name="module_jupiter.physical2"></a>

### jupiter.physical2(jde) ⇒ <code>Array</code>
Physical2 computes quantities for physical observations of Jupiter.

Results are less accurate than with Physical().
All angular results in radians.

**Kind**: static method of [<code>jupiter</code>](#module_jupiter)  
**Returns**: <code>Array</code> - {number} DS - Planetocentric declination of the Sun.
   {number} DE - Planetocentric declination of the Earth.
   {number} ω1 - Longitude of the System I central meridian of the illuminated disk,
                 as seen from Earth.
   {number} ω2 - Longitude of the System II central meridian of the illuminated disk,
                 as seen from Earth.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_jupitermoons"></a>

## jupitermoons
**License**: MIT  
**Copyright**: 2016 commenthol  

* [jupitermoons](#module_jupitermoons)
    * _static_
        * [.positions(jde)](#module_jupitermoons.positions) ⇒ <code>Array</code>
        * [.e5(jde, earth, jupiter, [pos])](#module_jupitermoons.e5) ⇒ <code>Array</code>
    * _inner_
        * [~XY(x, y)](#module_jupitermoons..XY)

<a name="module_jupitermoons.positions"></a>

### jupitermoons.positions(jde) ⇒ <code>Array</code>
Positions computes positions of moons of Jupiter.

Returned coordinates are in units of Jupiter radii.

**Kind**: static method of [<code>jupitermoons</code>](#module_jupitermoons)  
**Returns**: <code>Array</code> - x, y - coordinates of the 4 Satellites of jupiter  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_jupitermoons.e5"></a>

### jupitermoons.e5(jde, earth, jupiter, [pos]) ⇒ <code>Array</code>
Positions computes positions of moons of Jupiter.

High accuracy method based on theory "E5"  Results returned in
argument pos, which must not be undefined.  Returned coordinates in units
of Jupiter radii.

**Kind**: static method of [<code>jupitermoons</code>](#module_jupitermoons)  
**Returns**: <code>Array</code> - x, y - coordinates of the 4 Satellites of jupiter  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 Planet earth |
| jupiter | <code>planetposition.Planet</code> | VSOP87 Planet jupiter |
| [pos] | <code>Array</code> | reference to array of positions (same as return value) |

<a name="module_jupitermoons..XY"></a>

### jupitermoons~XY(x, y)
XY used for returning coordinates of moons.

**Kind**: inner method of [<code>jupitermoons</code>](#module_jupitermoons)  

| Param | Type | Description |
| --- | --- | --- |
| x | <code>number</code> | in units of Jupiter radii |
| y | <code>number</code> | in units of Jupiter radii |

<a name="module_kepler"></a>

## kepler
**License**: MIT  
**Copyright**: 2016 commenthol  

* [kepler](#module_kepler)
    * [.trueAnomaly(e, E)](#module_kepler.trueAnomaly) ⇒
    * [.radius(e, E, a)](#module_kepler.radius) ⇒ <code>number</code>
    * [.kepler1(e, m, places)](#module_kepler.kepler1) ⇒ <code>number</code>
    * [.kepler2(e, m, places)](#module_kepler.kepler2) ⇒ <code>number</code>
    * [.kepler2a(e, m, places)](#module_kepler.kepler2a) ⇒ <code>number</code>
    * [.kepler2b(e, m, places)](#module_kepler.kepler2b) ⇒ <code>number</code>
    * [.kepler3(e, m)](#module_kepler.kepler3) ⇒ <code>number</code>
    * [.kepler4(e, m)](#module_kepler.kepler4) ⇒ <code>number</code>

<a name="module_kepler.trueAnomaly"></a>

### kepler.trueAnomaly(e, E) ⇒
True returns true anomaly ν for given eccentric anomaly E.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: true anomaly ν in radians.  

| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| E | <code>number</code> | eccentric anomaly in radians. |

<a name="module_kepler.radius"></a>

### kepler.radius(e, E, a) ⇒ <code>number</code>
Radius returns radius distance r for given eccentric anomaly E.

Result unit is the unit of semimajor axis a (typically AU.)

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - radius distance in unit of `a`  

| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| E | <code>number</code> | eccentric anomaly in radians |
| a | <code>number</code> | semimajor axis |

<a name="module_kepler.kepler1"></a>

### kepler.kepler1(e, m, places) ⇒ <code>number</code>
Kepler1 solves Kepler's equation by iteration.

The iterated formula is

 E1 = m + e * sin(E0)

For some vaues of e and M it will fail to converge and the
function will return an error.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |
| places | <code>number</code> | (int) desired number of decimal places in the result |

<a name="module_kepler.kepler2"></a>

### kepler.kepler2(e, m, places) ⇒ <code>number</code>
Kepler2 solves Kepler's equation by iteration.

The iterated formula is

 E1 = E0 + (m + e * sin(E0) - E0) / (1 - e * cos(E0))

The function converges over a wider range of inputs than does Kepler1
but it also fails to converge for some values of e and M.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |
| places | <code>number</code> | (int) desired number of decimal places in the result |

<a name="module_kepler.kepler2a"></a>

### kepler.kepler2a(e, m, places) ⇒ <code>number</code>
Kepler2a solves Kepler's equation by iteration.

The iterated formula is the same as in Kepler2 but a limiting function
avoids divergence.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |
| places | <code>number</code> | (int) desired number of decimal places in the result |

<a name="module_kepler.kepler2b"></a>

### kepler.kepler2b(e, m, places) ⇒ <code>number</code>
Kepler2b solves Kepler's equation by iteration.

The iterated formula is the same as in Kepler2 but a (different) limiting
function avoids divergence.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |
| places | <code>number</code> | (int) desired number of decimal places in the result |

<a name="module_kepler.kepler3"></a>

### kepler.kepler3(e, m) ⇒ <code>number</code>
Kepler3 solves Kepler's equation by binary search.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |

<a name="module_kepler.kepler4"></a>

### kepler.kepler4(e, m) ⇒ <code>number</code>
Kepler4 returns an approximate solution to Kepler's equation.

It is valid only for small values of e.

**Kind**: static method of [<code>kepler</code>](#module_kepler)  
**Returns**: <code>number</code> - eccentric anomaly `E` in radians.  

| Param | Type | Description |
| --- | --- | --- |
| e | <code>number</code> | eccentricity |
| m | <code>number</code> | mean anomaly in radians |

<a name="module_line"></a>

## line
**License**: MIT  
**Copyright**: 2016 commenthol  

* [line](#module_line)
    * [.time(r1, d1, r2, d2, r3, d2, d3, t1, t5)](#module_line.time) ⇒ <code>Number</code>
    * [.angle()](#module_line.angle)
    * [.error()](#module_line.error)
    * [.angleError()](#module_line.angleError) ⇒ <code>Array.&lt;Number&gt;</code>

<a name="module_line.time"></a>

### line.time(r1, d1, r2, d2, r3, d2, d3, t1, t5) ⇒ <code>Number</code>
Time computes the time at which a moving body is on a straight line (great
circle) between two fixed points, such as stars.

Coordinates may be right ascensions and declinations or longitudes and
latitudes.  Fixed points are r1, d1, r2, d2.  Moving body is an ephemeris
of 5 rows, r3, d3, starting at time t1 and ending at time t5.  Time scale
is arbitrary.

**Kind**: static method of [<code>line</code>](#module_line)  
**Returns**: <code>Number</code> - time of alignment in Julian Days  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| r1 | <code>Number</code> | right ascension Coordinate 1 |
| d1 | <code>Number</code> | declination Coordinate 1 |
| r2 | <code>Number</code> | right ascension Coordinate 2 |
| d2 | <code>Number</code> | declination Coordinate 2 |
| r3 | <code>Number</code> | right ascension Coordinate 3 |
| d2 | <code>Number</code> | declination Coordinate 3 |
| d3 | <code>Array</code> | - |
| t1 | <code>Array</code> | time in Julian Days |
| t5 | <code>Array</code> | time in Julian Days |

<a name="module_line.angle"></a>

### line.angle()
Angle returns the angle between great circles defined by three points.

Coordinates may be right ascensions and declinations or longitudes and
latitudes.  If r1, d1, r2, d2 defines one line and r2, d2, r3, d3 defines
another, the result is the angle between the two lines.

Algorithm by Meeus.

**Kind**: static method of [<code>line</code>](#module_line)  
<a name="module_line.error"></a>

### line.error()
Error returns an error angle of three nearly co-linear points.

For the line defined by r1, d1, r2, d2, the result is the anglular distance
between that line and r0, d0.

Algorithm by Meeus.

**Kind**: static method of [<code>line</code>](#module_line)  
<a name="module_line.angleError"></a>

### line.angleError() ⇒ <code>Array.&lt;Number&gt;</code>
AngleError returns both an angle as in the function Angle, and an error
as in the function Error.

The algorithm is by B. Pessens.

**Kind**: static method of [<code>line</code>](#module_line)  
**Returns**: <code>Array.&lt;Number&gt;</code> - [ψ, ω]
 {Number} ψ - angle between great circles defined by three points.
 {Number} ω - error angle of three nearly co-linear points  
<a name="module_mars"></a>

## mars
**License**: MIT  
**Copyright**: 2016 commenthol  
<a name="module_mars.physical"></a>

### mars.physical(jde, earth, mars)
Physical computes quantities for physical observations of Mars.

Results:
 DE  planetocentric declination of the Earth.
 DS  planetocentric declination of the Sun.
 ω   Areographic longitude of the central meridian, as seen from Earth.
 P   Geocentric position angle of Mars' northern rotation pole.
 Q   Position angle of greatest defect of illumination.
 d   Apparent diameter of Mars.
 k   Illuminated fraction of the disk.
 q   Greatest defect of illumination.

All angular results (all results except k) are in radians.

**Kind**: static method of [<code>mars</code>](#module_mars)  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> |  |
| mars | <code>planetposition.Planet</code> |  |

<a name="module_moon"></a>

## moon
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moon](#module_moon)
    * [.Moon](#module_moon.Moon)
        * [.lib()](#module_moon.Moon+lib)
    * [.selenographic](#module_moon.selenographic)
    * [.physical(jde, earth)](#module_moon.physical) ⇒ <code>Array</code>
    * [.sunAltitude(cOnMoon, cSun)](#module_moon.sunAltitude) ⇒
    * [.sunrise(cOnMoon, jde, earth)](#module_moon.sunrise) ⇒
    * [.sunset(cOnMoon, jde, earth)](#module_moon.sunset) ⇒

<a name="module_moon.Moon"></a>

### moon.Moon
Quantities computed for a jde and used in computing return values of
physical().  Computations are broken into several methods to organize
the code.

**Kind**: static class of [<code>moon</code>](#module_moon)  
<a name="module_moon.Moon+lib"></a>

#### moon.lib()
lib() curiously serves for computing both librations and solar coordinates,
depending on the coordinates λ, β passed in.  Quantity A not described in
the book, but clearly depends on the λ, β of the current context and so
does not belong in the moon struct.  Instead just return it from optical
and pass it along to physical.

**Kind**: instance method of [<code>Moon</code>](#module_moon.Moon)  
<a name="module_moon.selenographic"></a>

### moon.selenographic
selenographic coordinates of some lunar features
Table 53.A

**Kind**: static constant of [<code>moon</code>](#module_moon)  
<a name="module_moon.physical"></a>

### moon.physical(jde, earth) ⇒ <code>Array</code>
Physical returns quantities useful for physical observation of the Moon.

Returned l, b are librations in selenographic longitude and latitude.
They represent combined optical and physical librations.  Topocentric
librations are not considered.

Returned P is the the position angle of the Moon's axis of rotation.

Returned l0, b0 are the selenographic coordinates of the Sun.

Returned values all in radians.

**Kind**: static method of [<code>moon</code>](#module_moon)  
**Returns**: <code>Array</code> - {base.Coord} cMoon - selenographic longitude, latitude of the Moon
   {number} P - position angle of the Moon's axis of rotation
   {base.Coord} cSun - selenographic longitude, latitude of the Sun.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 Planet Earth |

<a name="module_moon.sunAltitude"></a>

### moon.sunAltitude(cOnMoon, cSun) ⇒
SunAltitude returns altitude of the Sun above the lunar horizon.

**Kind**: static method of [<code>moon</code>](#module_moon)  
**Returns**: altitude in radians.  

| Param | Type | Description |
| --- | --- | --- |
| cOnMoon | <code>base.Coords</code> | selenographic longitude and latitude of a site on the Moon |
| cSun | <code>base.Coords</code> | selenographic coordinates of the Sun (as returned by physical(), for example.) |

<a name="module_moon.sunrise"></a>

### moon.sunrise(cOnMoon, jde, earth) ⇒
Sunrise returns time of sunrise for a point on the Moon near the given date.

**Kind**: static method of [<code>moon</code>](#module_moon)  
**Returns**: time of sunrise as a jde nearest the given jde.  

| Param | Type | Description |
| --- | --- | --- |
| cOnMoon | <code>base.Coord</code> | selenographic longitude and latitude of a site on the Moon |
| jde | <code>Number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 Planet Earth |

<a name="module_moon.sunset"></a>

### moon.sunset(cOnMoon, jde, earth) ⇒
Sunset returns time of sunset for a point on the Moon near the given date.

**Kind**: static method of [<code>moon</code>](#module_moon)  
**Returns**: time of sunset as a jde nearest the given jde.  

| Param | Type | Description |
| --- | --- | --- |
| cOnMoon | <code>base.Coords</code> | selenographic longitude and latitude of a site on the Moon |
| jde | <code>Number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 Planet Earth |

<a name="module_moonillum"></a>

## moonillum
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moonillum](#module_moonillum)
    * [.phaseAngleEquatorial(cMoon, cSun)](#module_moonillum.phaseAngleEquatorial) ⇒ <code>number</code>
    * [.phaseAngleEquatorial2(cMoon, cSun)](#module_moonillum.phaseAngleEquatorial2) ⇒ <code>number</code>
    * [.phaseAngleEcliptic(cMoon, cSun)](#module_moonillum.phaseAngleEcliptic) ⇒ <code>number</code>
    * [.phaseAngleEcliptic2(cMoon, cSun)](#module_moonillum.phaseAngleEcliptic2) ⇒ <code>number</code>
    * [.phaseAngle3()](#module_moonillum.phaseAngle3)

<a name="module_moonillum.phaseAngleEquatorial"></a>

### moonillum.phaseAngleEquatorial(cMoon, cSun) ⇒ <code>number</code>
phaseAngleEquatorial computes the phase angle of the Moon given equatorial coordinates.

**Kind**: static method of [<code>moonillum</code>](#module_moonillum)  
**Returns**: <code>number</code> - phase angle of the Moon in radians  

| Param | Type | Description |
| --- | --- | --- |
| cMoon | <code>base.Coord</code> | geocentric right ascension,  declination and distance to the Moon |
| cSun | <code>base.Coord</code> | coordinates and distance of the Sun |

<a name="module_moonillum.phaseAngleEquatorial2"></a>

### moonillum.phaseAngleEquatorial2(cMoon, cSun) ⇒ <code>number</code>
phaseAngleEquatorial2 computes the phase angle of the Moon given equatorial coordinates.

Less accurate than phaseAngleEquatorial.

Arguments α, δ are geocentric right ascension and declination of the Moon;
α0, δ0  are coordinates of the Sun.  Angles must be in radians.

**Kind**: static method of [<code>moonillum</code>](#module_moonillum)  
**Returns**: <code>number</code> - phase angle of the Moon in radians  

| Param | Type | Description |
| --- | --- | --- |
| cMoon | <code>base.Coord</code> | eocentric right ascension and declination of the Moon |
| cSun | <code>base.Coord</code> | coordinates of the Sun |

<a name="module_moonillum.phaseAngleEcliptic"></a>

### moonillum.phaseAngleEcliptic(cMoon, cSun) ⇒ <code>number</code>
phaseAngleEcliptic computes the phase angle of the Moon given ecliptic coordinates.

Distances must be in the same units as each other.

**Kind**: static method of [<code>moonillum</code>](#module_moonillum)  
**Returns**: <code>number</code> - phase angle of the Moon in radians  

| Param | Type | Description |
| --- | --- | --- |
| cMoon | <code>base.Coord</code> | geocentric longitude, latitude and distance to the Moon |
| cSun | <code>base.Coord</code> | longitude and distance to the Sun |

<a name="module_moonillum.phaseAngleEcliptic2"></a>

### moonillum.phaseAngleEcliptic2(cMoon, cSun) ⇒ <code>number</code>
phaseAngleEcliptic2 computes the phase angle of the Moon given ecliptic coordinates.

Less accurate than phaseAngleEcliptic.

Angles must be in radians.

**Kind**: static method of [<code>moonillum</code>](#module_moonillum)  
**Returns**: <code>number</code> - phase angle of the Moon in radians  

| Param | Type | Description |
| --- | --- | --- |
| cMoon | <code>base.Coord</code> | geocentric longitude, latitude of the Moon |
| cSun | <code>base.Coord</code> | longitude of the Sun |

<a name="module_moonillum.phaseAngle3"></a>

### moonillum.phaseAngle3()
phaseAngle3 computes the phase angle of the Moon given a julian day.

Less accurate than phaseAngle functions taking coordinates.

Result in radians.

**Kind**: static method of [<code>moonillum</code>](#module_moonillum)  
<a name="module_moonmaxdec"></a>

## moonmaxdec
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moonmaxdec](#module_moonmaxdec)
    * _static_
        * [.north()](#module_moonmaxdec.north)
        * [.south()](#module_moonmaxdec.south)
    * _inner_
        * [~nc](#module_moonmaxdec..nc)
        * [~sc](#module_moonmaxdec..sc)

<a name="module_moonmaxdec.north"></a>

### moonmaxdec.north()
North computes the maximum northern declination of the Moon near a given date.

Argument year is a decimal year specifying a date near the event.

Returned is the jde of the event nearest the given date and the declination
of the Moon at that time.

**Kind**: static method of [<code>moonmaxdec</code>](#module_moonmaxdec)  
<a name="module_moonmaxdec.south"></a>

### moonmaxdec.south()
South computes the maximum southern declination of the Moon near a given date.

Argument year is a decimal year specifying a date near the event.

Returned is the jde of the event nearest the given date and the declination
of the Moon at that time.

**Kind**: static method of [<code>moonmaxdec</code>](#module_moonmaxdec)  
<a name="module_moonmaxdec..nc"></a>

### moonmaxdec~nc
north coefficients

**Kind**: inner constant of [<code>moonmaxdec</code>](#module_moonmaxdec)  
<a name="module_moonmaxdec..sc"></a>

### moonmaxdec~sc
south coefficients

**Kind**: inner constant of [<code>moonmaxdec</code>](#module_moonmaxdec)  
<a name="module_moonnode"></a>

## moonnode
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moonnode](#module_moonnode)
    * [.ascending(year)](#module_moonnode.ascending) ⇒ <code>Number</code>
    * [.descending(year)](#module_moonnode.descending) ⇒ <code>Number</code>

<a name="module_moonnode.ascending"></a>

### moonnode.ascending(year) ⇒ <code>Number</code>
Ascending returns the date of passage of the Moon through an ascending node.

**Kind**: static method of [<code>moonnode</code>](#module_moonnode)  
**Returns**: <code>Number</code> - jde of the event nearest the given date.  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year specifying a date near the event. |

<a name="module_moonnode.descending"></a>

### moonnode.descending(year) ⇒ <code>Number</code>
Descending returns the date of passage of the Moon through a descending node.

**Kind**: static method of [<code>moonnode</code>](#module_moonnode)  
**Returns**: <code>Number</code> - jde of the event nearest the given date.  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year specifying a date near the event. |

<a name="module_moonphase"></a>

## moonphase
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moonphase](#module_moonphase)
    * _static_
        * [.meanLunarMonth](#module_moonphase.meanLunarMonth)
        * [.meanNew(year)](#module_moonphase.meanNew) ⇒ <code>Number</code>
        * [.meanFirst(year)](#module_moonphase.meanFirst) ⇒ <code>Number</code>
        * [.meanFull(year)](#module_moonphase.meanFull) ⇒ <code>Number</code>
        * [.meanLast(year)](#module_moonphase.meanLast) ⇒ <code>Number</code>
        * [.newMoon(year)](#module_moonphase.newMoon) ⇒ <code>Number</code>
        * [.first(year)](#module_moonphase.first) ⇒ <code>Number</code>
        * [.full(year)](#module_moonphase.full) ⇒ <code>Number</code>
        * [.last(year)](#module_moonphase.last) ⇒ <code>Number</code>
    * _inner_
        * [~snap()](#module_moonphase..snap)

<a name="module_moonphase.meanLunarMonth"></a>

### moonphase.meanLunarMonth
mean synodial lunar month

**Kind**: static constant of [<code>moonphase</code>](#module_moonphase)  
<a name="module_moonphase.meanNew"></a>

### moonphase.meanNew(year) ⇒ <code>Number</code>
MeanNew returns the jde of the mean New Moon nearest the given datthis.
The mean date is within 0.5 day of the true date of New Moon.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.meanFirst"></a>

### moonphase.meanFirst(year) ⇒ <code>Number</code>
MeanFirst returns the jde of the mean First Quarter Moon nearest the given datthis.
The mean date is within 0.5 day of the true date of First Quarter Moon.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.meanFull"></a>

### moonphase.meanFull(year) ⇒ <code>Number</code>
MeanFull returns the jde of the mean Full Moon nearest the given datthis.
The mean date is within 0.5 day of the true date of Full Moon.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.meanLast"></a>

### moonphase.meanLast(year) ⇒ <code>Number</code>
MeanLast returns the jde of the mean Last Quarter Moon nearest the given datthis.
The mean date is within 0.5 day of the true date of Last Quarter Moon.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.newMoon"></a>

### moonphase.newMoon(year) ⇒ <code>Number</code>
New returns the jde of New Moon nearest the given date.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.first"></a>

### moonphase.first(year) ⇒ <code>Number</code>
First returns the jde of First Quarter Moon nearest the given datthis.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.full"></a>

### moonphase.full(year) ⇒ <code>Number</code>
Full returns the jde of Full Moon nearest the given datthis.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase.last"></a>

### moonphase.last(year) ⇒ <code>Number</code>
Last returns the jde of Last Quarter Moon nearest the given datthis.

**Kind**: static method of [<code>moonphase</code>](#module_moonphase)  
**Returns**: <code>Number</code> - jde  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | decimal year |

<a name="module_moonphase..snap"></a>

### moonphase~snap()
snap returns k at specified quarter q nearest year y.

**Kind**: inner method of [<code>moonphase</code>](#module_moonphase)  
<a name="module_moonposition"></a>

## moonposition
**License**: MIT  
**Copyright**: 2016 commenthol  

* [moonposition](#module_moonposition)
    * [.parallax(distance)](#module_moonposition.parallax) ⇒ <code>Number</code>
    * [.position(jde)](#module_moonposition.position) ⇒ <code>base.Coord</code>
    * [.node(jde)](#module_moonposition.node) ⇒
    * [.perigee(jde)](#module_moonposition.perigee) ⇒
    * [.trueNode(jde)](#module_moonposition.trueNode) ⇒

<a name="module_moonposition.parallax"></a>

### moonposition.parallax(distance) ⇒ <code>Number</code>
parallax returns equatorial horizontal parallax of the Moon.

**Kind**: static method of [<code>moonposition</code>](#module_moonposition)  
**Returns**: <code>Number</code> - Result in radians.  

| Param | Type | Description |
| --- | --- | --- |
| distance | <code>Number</code> | distance between centers of the Earth and Moon, in km. |

<a name="module_moonposition.position"></a>

### moonposition.position(jde) ⇒ <code>base.Coord</code>
position returns geocentric location of the Moon.

Results are referenced to mean equinox of date and do not include
the effect of nutation.

**Kind**: static method of [<code>moonposition</code>](#module_moonposition)  
**Returns**: <code>base.Coord</code> - {number} lon - Geocentric longitude λ, in radians.
 {number} lat - Geocentric latitude β, in radians.
 {number} range - Distance Δ between centers of the Earth and Moon, in km.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_moonposition.node"></a>

### moonposition.node(jde) ⇒
Node returns longitude of the mean ascending node of the lunar orbit.

**Kind**: static method of [<code>moonposition</code>](#module_moonposition)  
**Returns**: result in radians.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_moonposition.perigee"></a>

### moonposition.perigee(jde) ⇒
perigee returns longitude of perigee of the lunar orbit.

**Kind**: static method of [<code>moonposition</code>](#module_moonposition)  
**Returns**: result in radians.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_moonposition.trueNode"></a>

### moonposition.trueNode(jde) ⇒
trueNode returns longitude of the true ascending node.

That is, the node of the instantaneous lunar orbit.

**Kind**: static method of [<code>moonposition</code>](#module_moonposition)  
**Returns**: result in radians.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_nearparabolic"></a>

## nearparabolic
**License**: MIT  
**Copyright**: 2016 commenthol  

* [nearparabolic](#module_nearparabolic)
    * [.Elements](#module_nearparabolic.Elements)
        * [new exports.Elements(timeP, pDis, ecc)](#new_module_nearparabolic.Elements_new)
        * [.anomalyDistance()](#module_nearparabolic.Elements+anomalyDistance)

<a name="module_nearparabolic.Elements"></a>

### nearparabolic.Elements
Elements holds orbital elements for near-parabolic orbits.

**Kind**: static class of [<code>nearparabolic</code>](#module_nearparabolic)  

* [.Elements](#module_nearparabolic.Elements)
    * [new exports.Elements(timeP, pDis, ecc)](#new_module_nearparabolic.Elements_new)
    * [.anomalyDistance()](#module_nearparabolic.Elements+anomalyDistance)

<a name="new_module_nearparabolic.Elements_new"></a>

#### new exports.Elements(timeP, pDis, ecc)

| Param | Type | Description |
| --- | --- | --- |
| timeP | <code>Number</code> | time of Perihelion, T |
| pDis | <code>Number</code> | Perihelion distance, q |
| ecc | <code>Number</code> | eccentricity, e |

<a name="module_nearparabolic.Elements+anomalyDistance"></a>

#### elements.anomalyDistance()
AnomalyDistance returns true anomaly and distance for near-parabolic orbits.

True anomaly ν returned in radians. Distance r returned in AU.
An error is returned if the algorithm fails to converge.

**Kind**: instance method of [<code>Elements</code>](#module_nearparabolic.Elements)  
<a name="module_node"></a>

## node
**License**: MIT  
**Copyright**: 2016 commenthol  

* [node](#module_node)
    * [.ellipticAscending()](#module_node.ellipticAscending)
    * [.ellipticDescending()](#module_node.ellipticDescending)
    * [.parabolicAscending()](#module_node.parabolicAscending)
    * [.parabolicDescending()](#module_node.parabolicDescending)

<a name="module_node.ellipticAscending"></a>

### node.ellipticAscending()
EllipticAscending computes time and distance of passage through the ascending node of a body in an elliptical orbit.

Argument axis is semimajor axis in AU, ecc is eccentricity, argP is argument
of perihelion in radians, timeP is time of perihelion as a jd.

Result is jde of the event and distance from the sun in AU.

**Kind**: static method of [<code>node</code>](#module_node)  
<a name="module_node.ellipticDescending"></a>

### node.ellipticDescending()
EllipticAscending computes time and distance of passage through the descending node of a body in an elliptical orbit.

Argument axis is semimajor axis in AU, ecc is eccentricity, argP is argument
of perihelion in radians, timeP is time of perihelion as a jd.

Result is jde of the event and distance from the sun in AU.

**Kind**: static method of [<code>node</code>](#module_node)  
<a name="module_node.parabolicAscending"></a>

### node.parabolicAscending()
ParabolicAscending computes time and distance of passage through the ascending node of a body in a parabolic orbit.

Argument q is perihelion distance in AU, argP is argument of perihelion
in radians, timeP is time of perihelion as a jd.

Result is jde of the event and distance from the sun in AU.

**Kind**: static method of [<code>node</code>](#module_node)  
<a name="module_node.parabolicDescending"></a>

### node.parabolicDescending()
ParabolicDescending computes time and distance of passage through the descending node of a body in a parabolic orbit.

Argument q is perihelion distance in AU, argP is argument of perihelion
in radians, timeP is time of perihelion as a jd.

Result is jde of the event and distance from the sun in AU.

**Kind**: static method of [<code>node</code>](#module_node)  
<a name="module_nutation"></a>

## nutation
**License**: MIT  
**Copyright**: 2016 commenthol  

* [nutation](#module_nutation)
    * [.nutation(jde)](#module_nutation.nutation) ⇒ <code>Array.&lt;number&gt;</code>
    * [.approxNutation(jde)](#module_nutation.approxNutation) ⇒ <code>Array.&lt;number&gt;</code>
    * [.meanObliquity(jde)](#module_nutation.meanObliquity) ⇒ <code>number</code>
    * [.meanObliquityLaskar(jde)](#module_nutation.meanObliquityLaskar) ⇒ <code>number</code>
    * [.nutationInRA(jde)](#module_nutation.nutationInRA) ⇒ <code>number</code>

<a name="module_nutation.nutation"></a>

### nutation.nutation(jde) ⇒ <code>Array.&lt;number&gt;</code>
Nutation returns nutation in longitude (Δψ) and nutation in obliquity (Δε)
for a given JDE.

JDE = UT + ΔT, see package.

Computation is by 1980 IAU theory, with terms < .0003″ neglected.

Result units are radians.

**Kind**: static method of [<code>nutation</code>](#module_nutation)  
**Returns**: <code>Array.&lt;number&gt;</code> - [Δψ, Δε] - [longitude, obliquity] in radians  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_nutation.approxNutation"></a>

### nutation.approxNutation(jde) ⇒ <code>Array.&lt;number&gt;</code>
ApproxNutation returns a fast approximation of nutation in longitude (Δψ)
and nutation in obliquity (Δε) for a given JDE.

Accuracy is 0.5″ in Δψ, 0.1″ in Δε.

Result units are radians.

**Kind**: static method of [<code>nutation</code>](#module_nutation)  
**Returns**: <code>Array.&lt;number&gt;</code> - [Δψ, Δε] - [longitude, obliquity] in radians  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_nutation.meanObliquity"></a>

### nutation.meanObliquity(jde) ⇒ <code>number</code>
MeanObliquity returns mean obliquity (ε₀) following the IAU 1980
polynomial.

Accuracy is 1″ over the range 1000 to 3000 years and 10″ over the range
0 to 4000 years.

Result unit is radians.

**Kind**: static method of [<code>nutation</code>](#module_nutation)  
**Returns**: <code>number</code> - mean obliquity (ε₀)  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_nutation.meanObliquityLaskar"></a>

### nutation.meanObliquityLaskar(jde) ⇒ <code>number</code>
MeanObliquityLaskar returns mean obliquity (ε₀) following the Laskar
1986 polynomial.

Accuracy over the range 1000 to 3000 years is .01″.

Accuracy over the valid date range of -8000 to +12000 years is
"a few seconds."

Result unit is radians.

**Kind**: static method of [<code>nutation</code>](#module_nutation)  
**Returns**: <code>number</code> - mean obliquity (ε₀)  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_nutation.nutationInRA"></a>

### nutation.nutationInRA(jde) ⇒ <code>number</code>
NutationInRA returns "nutation in right ascension" or "equation of the
equinoxes."

Result is an angle in radians.

**Kind**: static method of [<code>nutation</code>](#module_nutation)  
**Returns**: <code>number</code> - nutation in right ascension  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |

<a name="module_parabolic"></a>

## parabolic
**License**: MIT  
**Copyright**: 2016 commenthol  

* [parabolic](#module_parabolic)
    * [.Elements](#module_parabolic.Elements)
        * [new exports.Elements(timeP, pDis)](#new_module_parabolic.Elements_new)
        * [.anomalyDistance(jde)](#module_parabolic.Elements+anomalyDistance) ⇒ <code>Object</code>

<a name="module_parabolic.Elements"></a>

### parabolic.Elements
Elements holds parabolic elements needed for computing true anomaly and distance.

**Kind**: static class of [<code>parabolic</code>](#module_parabolic)  

* [.Elements](#module_parabolic.Elements)
    * [new exports.Elements(timeP, pDis)](#new_module_parabolic.Elements_new)
    * [.anomalyDistance(jde)](#module_parabolic.Elements+anomalyDistance) ⇒ <code>Object</code>

<a name="new_module_parabolic.Elements_new"></a>

#### new exports.Elements(timeP, pDis)

| Param | Type | Description |
| --- | --- | --- |
| timeP | <code>Number</code> | time of perihelion, T |
| pDis | <code>Number</code> | perihelion distance, q |

<a name="module_parabolic.Elements+anomalyDistance"></a>

#### elements.anomalyDistance(jde) ⇒ <code>Object</code>
AnomalyDistance returns true anomaly and distance of a body in a parabolic orbit of the Sun.

**Kind**: instance method of [<code>Elements</code>](#module_parabolic.Elements)  
**Returns**: <code>Object</code> - {ano, dist}
  {Number} ano - True anomaly ν in radians.
  {Number} dist - Distance r returned in AU.  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_parallactic"></a>

## parallactic
**License**: MIT  
**Copyright**: 2016 commenthol  

* [parallactic](#module_parallactic)
    * [.parallacticAngle()](#module_parallactic.parallacticAngle)
    * [.parallacticAngleOnHorizon()](#module_parallactic.parallacticAngleOnHorizon)
    * [.eclipticAtHorizon()](#module_parallactic.eclipticAtHorizon)
    * [.eclipticAtEquator()](#module_parallactic.eclipticAtEquator)
    * [.diurnalPathAtHorizon()](#module_parallactic.diurnalPathAtHorizon)

<a name="module_parallactic.parallacticAngle"></a>

### parallactic.parallacticAngle()
ParallacticAngle returns parallactic angle of a celestial object.

 φ is geographic latitude of observer.
 δ is declination of observed object.
 H is hour angle of observed object.

All angles including result are in radians.

**Kind**: static method of [<code>parallactic</code>](#module_parallactic)  
<a name="module_parallactic.parallacticAngleOnHorizon"></a>

### parallactic.parallacticAngleOnHorizon()
ParallacticAngleOnHorizon is a special case of ParallacticAngle.

The hour angle is not needed as an input and the math inside simplifies.

**Kind**: static method of [<code>parallactic</code>](#module_parallactic)  
<a name="module_parallactic.eclipticAtHorizon"></a>

### parallactic.eclipticAtHorizon()
EclipticAtHorizon computes how the plane of the ecliptic intersects
the horizon at a given local sidereal time as observed from a given
geographic latitude.

 ε is obliquity of the ecliptic.
 φ is geographic latitude of observer.
 θ is local sidereal time expressed as an hour angle.

 λ1 and λ2 are ecliptic longitudes where the ecliptic intersects the horizon.
 I is the angle at which the ecliptic intersects the horizon.

All angles, arguments and results, are in radians.

**Kind**: static method of [<code>parallactic</code>](#module_parallactic)  
<a name="module_parallactic.eclipticAtEquator"></a>

### parallactic.eclipticAtEquator()
EclipticAtEquator computes the angle between the ecliptic and the parallels
of ecliptic latitude at a given ecliptic longitude.

(The function name EclipticAtEquator is for consistency with the Meeus text,
and works if you consider the equator a nominal parallel of latitude.)

 λ is ecliptic longitude.
 ε is obliquity of the ecliptic.

All angles in radians.

**Kind**: static method of [<code>parallactic</code>](#module_parallactic)  
<a name="module_parallactic.diurnalPathAtHorizon"></a>

### parallactic.diurnalPathAtHorizon()
DiurnalPathAtHorizon computes the angle of the path a celestial object
relative to the horizon at the time of its rising or setting.

 δ is declination of the object.
 φ is geographic latitude of observer.

All angles in radians.

**Kind**: static method of [<code>parallactic</code>](#module_parallactic)  
<a name="module_parallax"></a>

## parallax
**License**: MIT  
**Copyright**: 2016 commenthol  

* [parallax](#module_parallax)
    * [.horizontal(Δ)](#module_parallax.horizontal) ⇒ <code>number</code>
    * [.topocentric(c, ρsφ, ρcφ, lon, jde)](#module_parallax.topocentric) ⇒ <code>base.Coord</code>
    * [.topocentric2(c, ρsφ, ρcφ, lon, jde)](#module_parallax.topocentric2) ⇒ <code>base.Coord</code>
    * [.topocentric3(c, ρsφ, ρcφ, lon, jde)](#module_parallax.topocentric3) ⇒ <code>Array</code>
    * [.topocentricEcliptical(c, s, φ, h, ε, θ, π)](#module_parallax.topocentricEcliptical) ⇒ <code>Array</code>

<a name="module_parallax.horizontal"></a>

### parallax.horizontal(Δ) ⇒ <code>number</code>
Horizontal returns equatorial horizontal parallax of a body.

**Kind**: static method of [<code>parallax</code>](#module_parallax)  
**Returns**: <code>number</code> - parallax in radians.  

| Param | Type | Description |
| --- | --- | --- |
| Δ | <code>number</code> | distance in AU. |

<a name="module_parallax.topocentric"></a>

### parallax.topocentric(c, ρsφ, ρcφ, lon, jde) ⇒ <code>base.Coord</code>
Topocentric returns topocentric positions including parallax.

Arguments α, δ are geocentric right ascension and declination in radians.
Δ is distance to the observed object in AU. ρsφ_, ρcφ_ are parallax
constants (see package globe.) lon is geographic longitude of the observer,
jde is time of observation.

**Kind**: static method of [<code>parallax</code>](#module_parallax)  
**Returns**: <code>base.Coord</code> - observed topocentric ra and dec in radians.  

| Param | Type | Description |
| --- | --- | --- |
| c | <code>base.Coord</code> | geocentric right ascension and declination in radians |
| ρsφ | <code>number</code> | parallax constants (see package globe.) |
| ρcφ | <code>number</code> | parallax constants (see package globe.) |
| lon | <code>number</code> | geographic longitude of the observer (measured positively westwards!) |
| jde | <code>number</code> | time of observation |

<a name="module_parallax.topocentric2"></a>

### parallax.topocentric2(c, ρsφ, ρcφ, lon, jde) ⇒ <code>base.Coord</code>
Topocentric2 returns topocentric corrections including parallax.

This function implements the "non-rigorous" method descripted in the text.

Note that results are corrections, not corrected coordinates.

**Kind**: static method of [<code>parallax</code>](#module_parallax)  
**Returns**: <code>base.Coord</code> - observed topocentric ra and dec in radians.  

| Param | Type | Description |
| --- | --- | --- |
| c | <code>base.Coord</code> | geocentric right ascension and declination in radians |
| ρsφ | <code>number</code> | parallax constants (see package globe.) |
| ρcφ | <code>number</code> | parallax constants (see package globe.) |
| lon | <code>number</code> | geographic longitude of the observer (measured positively westwards!) |
| jde | <code>number</code> | time of observation |

<a name="module_parallax.topocentric3"></a>

### parallax.topocentric3(c, ρsφ, ρcφ, lon, jde) ⇒ <code>Array</code>
Topocentric3 returns topocentric hour angle and declination including parallax.

This function implements the "alternative" method described in the text.
The method should be similarly rigorous to that of Topocentric() and results
should be virtually consistent.

**Kind**: static method of [<code>parallax</code>](#module_parallax)  
**Returns**: <code>Array</code> - {number} H_ - topocentric hour angle
   {number} δ_ - topocentric declination  

| Param | Type | Description |
| --- | --- | --- |
| c | <code>base.Coord</code> | geocentric right ascension and declination in radians |
| ρsφ | <code>number</code> | parallax constants (see package globe.) |
| ρcφ | <code>number</code> | parallax constants (see package globe.) |
| lon | <code>number</code> | geographic longitude of the observer (measured positively westwards!) |
| jde | <code>number</code> | time of observation |

<a name="module_parallax.topocentricEcliptical"></a>

### parallax.topocentricEcliptical(c, s, φ, h, ε, θ, π) ⇒ <code>Array</code>
TopocentricEcliptical returns topocentric ecliptical coordinates including parallax.

Arguments `c` are geocentric ecliptical longitude and latitude of a body,
s is its geocentric semidiameter. φ, h are the observer's latitude and
and height above the ellipsoid in meters.  ε is the obliquity of the
ecliptic, θ is local sidereal time, π is equatorial horizontal parallax
of the body (see Horizonal()).

All angular parameters and results are in radians.

**Kind**: static method of [<code>parallax</code>](#module_parallax)  
**Returns**: <code>Array</code> - {number} λ_ - observed topocentric longitude
   {number} β_ - observed topocentric latitude
   {number} s_ - observed topocentric semidiameter  

| Param | Type | Description |
| --- | --- | --- |
| c | <code>base.Coord</code> | geocentric right ascension and declination in radians |
| s | <code>number</code> | geocentric semidiameter of `c` |
| φ | <code>number</code> | observer's latitude |
| h | <code>number</code> | observer's height above the ellipsoid in meters |
| ε | <code>number</code> | is the obliquity of the ecliptic |
| θ | <code>number</code> | local sidereal time |
| π | <code>number</code> | equatorial horizontal parallax of the body |

<a name="module_perihelion"></a>

## perihelion
**License**: MIT  
**Copyright**: 2016 commenthol  

* [perihelion](#module_perihelion)
    * _static_
        * [.perihelion(p, y)](#module_perihelion.perihelion) ⇒ <code>Number</code>
        * [.aphelion(p, y)](#module_perihelion.aphelion) ⇒ <code>Number</code>
        * [.perihelion2(planet, year, precision, [cb])](#module_perihelion.perihelion2) ⇒ <code>Array</code>
        * [.aphelion2(planet, year, precision, [cb])](#module_perihelion.aphelion2) ⇒ <code>Array</code>
    * _inner_
        * [~planets](#module_perihelion..planets)

<a name="module_perihelion.perihelion"></a>

### perihelion.perihelion(p, y) ⇒ <code>Number</code>
Perihelion returns an approximate jde of the perihelion event nearest the given time.

**Kind**: static method of [<code>perihelion</code>](#module_perihelion)  
**Returns**: <code>Number</code> - jde - time of the event  

| Param | Type | Description |
| --- | --- | --- |
| p | <code>perihelion.NAME</code> | planet constant from above |
| y | <code>Number</code> | year number indicating a time near the perihelion event. |

<a name="module_perihelion.aphelion"></a>

### perihelion.aphelion(p, y) ⇒ <code>Number</code>
Aphelion returns an approximate jde of the aphelion event nearest the given time.

**Kind**: static method of [<code>perihelion</code>](#module_perihelion)  
**Returns**: <code>Number</code> - jde - time of the event  

| Param | Type | Description |
| --- | --- | --- |
| p | <code>perihelion.NAME</code> | planet constant from above |
| y | <code>Number</code> | year number indicating a time near the aphelion event. |

<a name="module_perihelion.perihelion2"></a>

### perihelion.perihelion2(planet, year, precision, [cb]) ⇒ <code>Array</code>
Perihelion2 returns the perihelion event nearest the given time.

**Kind**: static method of [<code>perihelion</code>](#module_perihelion)  
**Returns**: <code>Array</code> - [jde, r]
  {Number} jde - time of the event
  {Number} r - the distance of the planet from the Sun in AU.  

| Param | Type | Description |
| --- | --- | --- |
| planet | <code>planetposition.Planet</code> | VSOP87 planet (EMBary is not allowed) |
| year | <code>Number</code> | (float) decimal year number near the perihelion event |
| precision | <code>Number</code> | desired precision of the time result, in days |
| [cb] | <code>function</code> | callback function for asynchronous processing `cb([jde, r])` |

<a name="module_perihelion.aphelion2"></a>

### perihelion.aphelion2(planet, year, precision, [cb]) ⇒ <code>Array</code>
Aphelion2 returns the aphelion event nearest the given time.

**Kind**: static method of [<code>perihelion</code>](#module_perihelion)  
**Returns**: <code>Array</code> - [jde, r]
  {Number} jde - time of the event
  {Number} r - the distance of the planet from the Sun in AU.  

| Param | Type | Description |
| --- | --- | --- |
| planet | <code>planetposition.Planet</code> | VSOP87 planet (EMBary is not allowed) |
| year | <code>Number</code> | (float) decimal year number near the perihelion event |
| precision | <code>Number</code> | desired precision of the time result, in days |
| [cb] | <code>function</code> | callback function for asynchronous processing `cb([jde, r])` |

<a name="module_perihelion..planets"></a>

### perihelion~planets
Planet constants for first argument of Perihelion and Aphelion functions.

**Kind**: inner constant of [<code>perihelion</code>](#module_perihelion)  
<a name="module_planetary"></a>

## planetary
**License**: MIT  
**Copyright**: 2016 commenthol  

* [planetary](#module_planetary)
    * _static_
        * [.mean()](#module_planetary.mean)
        * [.sum()](#module_planetary.sum)
        * [.ms()](#module_planetary.ms)
        * [.mercuryInfConj()](#module_planetary.mercuryInfConj)
        * [.mercurySupConj()](#module_planetary.mercurySupConj)
        * [.venusInfConj()](#module_planetary.venusInfConj)
        * [.marsOpp()](#module_planetary.marsOpp)
        * [.sumA()](#module_planetary.sumA)
        * [.msa()](#module_planetary.msa)
        * [.jupiterOpp()](#module_planetary.jupiterOpp)
        * [.saturnOpp()](#module_planetary.saturnOpp)
        * [.saturnConj()](#module_planetary.saturnConj)
        * [.uranusOpp()](#module_planetary.uranusOpp)
        * [.neptuneOpp()](#module_planetary.neptuneOpp)
        * [.el()](#module_planetary.el)
        * [.mercuryEastElongation()](#module_planetary.mercuryEastElongation)
        * [.mercuryWestElongation()](#module_planetary.mercuryWestElongation)
    * _inner_
        * [~micA](#module_planetary..micA)
        * [~micB](#module_planetary..micB)
        * [~mscB](#module_planetary..mscB)
        * [~vicB](#module_planetary..vicB)
        * [~moB](#module_planetary..moB)
        * [~joB](#module_planetary..joB)
        * [~soB](#module_planetary..soB)
        * [~scB](#module_planetary..scB)
        * [~uoB](#module_planetary..uoB)
        * [~noB](#module_planetary..noB)
        * [~met](#module_planetary..met)
        * [~mee](#module_planetary..mee)
        * [~mwt](#module_planetary..mwt)
        * [~mwe](#module_planetary..mwe)
        * [~ms2](#module_planetary..ms2)
        * [~Ca()](#module_planetary..Ca)
        * [~Caa()](#module_planetary..Caa)

<a name="module_planetary.mean"></a>

### planetary.mean()
Mean computes some intermediate values for a mean planetary configuration
given a year and a row of coefficients from Table 36.A, p. 250.0

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.sum"></a>

### planetary.sum()
Sum computes a sum of periodic terms.

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.ms"></a>

### planetary.ms()
ms returns a mean time corrected by a sum.

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.mercuryInfConj"></a>

### planetary.mercuryInfConj()
MercuryInfConj returns the time of an inferior conjunction of Mercury.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.mercurySupConj"></a>

### planetary.mercurySupConj()
MercurySupConj returns the time of a superior conjunction of Mercury.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.venusInfConj"></a>

### planetary.venusInfConj()
VenusInfConj returns the time of an inferior conjunction of Venus.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.marsOpp"></a>

### planetary.marsOpp()
MarsOpp returns the time of an opposition of Mars.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.sumA"></a>

### planetary.sumA()
SumA computes the sum of periodic terms with "additional angles"

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.msa"></a>

### planetary.msa()
Msa returns a mean time corrected by a sum.

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.jupiterOpp"></a>

### planetary.jupiterOpp()
JupiterOpp returns the time of an opposition of Jupiter.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.saturnOpp"></a>

### planetary.saturnOpp()
SaturnOpp returns the time of an opposition of Saturn.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.saturnConj"></a>

### planetary.saturnConj()
SaturnConj returns the time of a conjunction of Saturn.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.uranusOpp"></a>

### planetary.uranusOpp()
UranusOpp returns the time of an opposition of Uranus.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.neptuneOpp"></a>

### planetary.neptuneOpp()
NeptuneOpp returns the time of an opposition of Neptune.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.el"></a>

### planetary.el()
El computes time and elongation of a greatest elongation event.

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.mercuryEastElongation"></a>

### planetary.mercuryEastElongation()
MercuryEastElongation returns the time and elongation of a greatest eastern elongation of Mercury.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary.mercuryWestElongation"></a>

### planetary.mercuryWestElongation()
MercuryWestElongation returns the time and elongation of a greatest western elongation of Mercury.

Result is time (as a jde) of the event nearest the given time (as a
decimal year.)

**Kind**: static method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..micA"></a>

### planetary~micA
Table 36.A, p. 250

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..micB"></a>

### planetary~micB
Mercury inferior conjunction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..mscB"></a>

### planetary~mscB
Mercury superior conjunction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..vicB"></a>

### planetary~vicB
Venus inferior conjunction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..moB"></a>

### planetary~moB
Mars opposition

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..joB"></a>

### planetary~joB
Jupiter opposition

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..soB"></a>

### planetary~soB
Saturn opposition

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..scB"></a>

### planetary~scB
Saturn conjunction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..uoB"></a>

### planetary~uoB
Uranus opposition

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..noB"></a>

### planetary~noB
Neptune opposition [

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..met"></a>

### planetary~met
Mercury east time correction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..mee"></a>

### planetary~mee
Mercury east elongation

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..mwt"></a>

### planetary~mwt
Mercury west time correction

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..mwe"></a>

### planetary~mwe
Mercury west elongation

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..ms2"></a>

### planetary~ms2
Mars Station 2

**Kind**: inner constant of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..Ca"></a>

### planetary~Ca()
ca holds coefficients from one line of table 36.A, p. 250

**Kind**: inner method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetary..Caa"></a>

### planetary~Caa()
caa holds coefficients for "additional angles" for outer planets
as given on p. 251

**Kind**: inner method of [<code>planetary</code>](#module_planetary)  
<a name="module_planetelements"></a>

## planetelements
**License**: MIT  
**Copyright**: 2016 commenthol  

* [planetelements](#module_planetelements)
    * _static_
        * [.Elements(lon, axis, ecc, inc, node, peri)](#module_planetelements.Elements)
        * [.mean()](#module_planetelements.mean)
        * [.inc()](#module_planetelements.inc)
        * [.node()](#module_planetelements.node)
    * _inner_
        * [~cMean](#module_planetelements..cMean)

<a name="module_planetelements.Elements"></a>

### planetelements.Elements(lon, axis, ecc, inc, node, peri)
Elements contains orbital elements as returned by functions in this package.

Some other elements easily derived from these are

 Mean Anomolay, M = Lon - Peri
 Argument of Perihelion, ω = Peri - Node

**Kind**: static method of [<code>planetelements</code>](#module_planetelements)  

| Param | Type | Description |
| --- | --- | --- |
| lon | <code>Number</code> | mean longitude, L |
| axis | <code>Number</code> | semimajor axis, a |
| ecc | <code>Number</code> | eccentricity, e |
| inc | <code>Number</code> | inclination, i |
| node | <code>Number</code> | longitude of ascending node, Ω |
| peri | <code>Number</code> | longitude of perihelion, ϖ (Meeus likes π better) |

<a name="module_planetelements.mean"></a>

### planetelements.mean()
Mean returns mean orbital elements for a planet

Argument p must be a planet const as defined above, argument e is
a result parameter.  A valid non-undefined pointer to an Elements struct
must be passed in.

Results are referenced to mean dynamical ecliptic and equinox of date.

Semimajor axis is in AU, angular elements are in radians.

**Kind**: static method of [<code>planetelements</code>](#module_planetelements)  
<a name="module_planetelements.inc"></a>

### planetelements.inc()
Inc returns mean inclination for a planet at a date.

Result is the same as the Inc field returned by function Mean.  That is,
radians, referenced to mean dynamical ecliptic and equinox of date.

**Kind**: static method of [<code>planetelements</code>](#module_planetelements)  
<a name="module_planetelements.node"></a>

### planetelements.node()
Node returns mean longitude of ascending node for a planet at a date.

Result is the same as the Node field returned by function Mean.  That is,
radians, referenced to mean dynamical ecliptic and equinox of date.

**Kind**: static method of [<code>planetelements</code>](#module_planetelements)  
<a name="module_planetelements..cMean"></a>

### planetelements~cMean
Table 31.A, p. 212

**Kind**: inner constant of [<code>planetelements</code>](#module_planetelements)  
<a name="module_planetposition"></a>

## planetposition
**License**: MIT  
**Copyright**: 2016 commenthol  
<a name="module_planetposition.toFK5"></a>

### planetposition.toFK5(lon, lat, jde) ⇒ <code>base.Coord</code>
ToFK5 converts ecliptic longitude and latitude from dynamical frame to FK5.

**Kind**: static method of [<code>planetposition</code>](#module_planetposition)  
**Returns**: <code>base.Coord</code> - {Number} lon - FK5 longitude
   {Number} lat - FK5 latitude  

| Param | Type | Description |
| --- | --- | --- |
| lon | <code>Number</code> | ecliptic longitude in radians |
| lat | <code>Number</code> | ecliptic latitude in radians |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_pluto"></a>

## pluto
**License**: MIT  
**Copyright**: 2016 commenthol  

* [pluto](#module_pluto)
    * [.heliocentric()](#module_pluto.heliocentric)
    * [.astrometric()](#module_pluto.astrometric)

<a name="module_pluto.heliocentric"></a>

### pluto.heliocentric()
Heliocentric returns J2000 heliocentric coordinates of Pluto.

Results l, b are solar longitude and latitude in radians.
Result r is distance in AU.

**Kind**: static method of [<code>pluto</code>](#module_pluto)  
<a name="module_pluto.astrometric"></a>

### pluto.astrometric()
Astrometric returns J2000 astrometric coordinates of Pluto.

**Kind**: static method of [<code>pluto</code>](#module_pluto)  
<a name="module_precess"></a>

## precess
**License**: MIT  
**Copyright**: 2016 commenthol  

* [precess](#module_precess)
    * [.Precessor](#module_precess.Precessor)
        * [new exports.Precessor(epochFrom, epochTo)](#new_module_precess.Precessor_new)
        * [.precess(eqFrom)](#module_precess.Precessor+precess) ⇒ <code>coord.Equatorial</code>
    * [.EclipticPrecessor](#module_precess.EclipticPrecessor)
        * [new exports.EclipticPrecessor(epochFrom, epochTo)](#new_module_precess.EclipticPrecessor_new)
        * [.precess(eclFrom, eclTo)](#module_precess.EclipticPrecessor+precess) ⇒ <code>coord.Ecliptic</code>
        * [.reduceElements(eFrom)](#module_precess.EclipticPrecessor+reduceElements) ⇒ <code>elementequinox.Elements</code>
    * [.approxAnnualPrecession(eqFrom, epochFrom, epochTo)](#module_precess.approxAnnualPrecession) ⇒ <code>Array</code>
    * [.mn(epochFrom, epochTo)](#module_precess.mn)
    * [.approxPosition(eqFrom, epochFrom, epochTo, mα, mδ)](#module_precess.approxPosition) ⇒ <code>coord.Equatorial</code>
    * [.position(eqFrom, eqTo, epochFrom, epochTo, mα, mδ)](#module_precess.position) ⇒ <code>coord.Equatorial</code>
    * [.eclipticPosition(eclFrom,, epochFrom, epochTo, mα, mδ)](#module_precess.eclipticPosition) ⇒ <code>coord.Ecliptic</code>
    * [.properMotion(mα, mδ, epoch, ecl)](#module_precess.properMotion) ⇒ <code>Array.&lt;Number&gt;</code>
    * [.properMotion3D(eqFrom,, epochFrom, r, mr, mα, mδ)](#module_precess.properMotion3D) ⇒ <code>coord.Equatorial</code>

<a name="module_precess.Precessor"></a>

### precess.Precessor
Precessor represents precession from one epoch to another.

Construct with NewPrecessor, then call method Precess.
After construction, Precess may be called multiple times to precess
different coordinates with the same initial and final epochs.

**Kind**: static class of [<code>precess</code>](#module_precess)  

* [.Precessor](#module_precess.Precessor)
    * [new exports.Precessor(epochFrom, epochTo)](#new_module_precess.Precessor_new)
    * [.precess(eqFrom)](#module_precess.Precessor+precess) ⇒ <code>coord.Equatorial</code>

<a name="new_module_precess.Precessor_new"></a>

#### new exports.Precessor(epochFrom, epochTo)
constructs a Precessor object and initializes it to precess
coordinates from epochFrom to epochTo.


| Param | Type |
| --- | --- |
| epochFrom | <code>Number</code> | 
| epochTo | <code>Number</code> | 

<a name="module_precess.Precessor+precess"></a>

#### precessor.precess(eqFrom) ⇒ <code>coord.Equatorial</code>
Precess precesses coordinates eqFrom, leaving result in eqTo.

**Kind**: instance method of [<code>Precessor</code>](#module_precess.Precessor)  
**Returns**: <code>coord.Equatorial</code> - eqTo  

| Param | Type |
| --- | --- |
| eqFrom | <code>coord.Equatorial</code> | 

<a name="module_precess.EclipticPrecessor"></a>

### precess.EclipticPrecessor
EclipticPrecessor represents precession from one epoch to another.

Construct with NewEclipticPrecessor, then call method Precess.
After construction, Precess may be called multiple times to precess
different coordinates with the same initial and final epochs.

**Kind**: static class of [<code>precess</code>](#module_precess)  

* [.EclipticPrecessor](#module_precess.EclipticPrecessor)
    * [new exports.EclipticPrecessor(epochFrom, epochTo)](#new_module_precess.EclipticPrecessor_new)
    * [.precess(eclFrom, eclTo)](#module_precess.EclipticPrecessor+precess) ⇒ <code>coord.Ecliptic</code>
    * [.reduceElements(eFrom)](#module_precess.EclipticPrecessor+reduceElements) ⇒ <code>elementequinox.Elements</code>

<a name="new_module_precess.EclipticPrecessor_new"></a>

#### new exports.EclipticPrecessor(epochFrom, epochTo)
constructs an EclipticPrecessor object and initializes
it to precess coordinates from epochFrom to epochTo.


| Param | Type |
| --- | --- |
| epochFrom | <code>Number</code> | 
| epochTo | <code>Number</code> | 

<a name="module_precess.EclipticPrecessor+precess"></a>

#### eclipticPrecessor.precess(eclFrom, eclTo) ⇒ <code>coord.Ecliptic</code>
EclipticPrecess precesses coordinates eclFrom, leaving result in eclTo.

The same struct may be used for eclFrom and eclTo.
EclTo is returned for convenience.

**Kind**: instance method of [<code>EclipticPrecessor</code>](#module_precess.EclipticPrecessor)  
**Returns**: <code>coord.Ecliptic</code> - [eclTo]  

| Param | Type |
| --- | --- |
| eclFrom | <code>coord.Ecliptic</code> | 
| eclTo | <code>coord.Ecliptic</code> | 

<a name="module_precess.EclipticPrecessor+reduceElements"></a>

#### eclipticPrecessor.reduceElements(eFrom) ⇒ <code>elementequinox.Elements</code>
ReduceElements reduces orbital elements of a solar system body from one
equinox to another.

This function is described in chapter 24, but is located in this
package so it can be a method of EclipticPrecessor.

**Kind**: instance method of [<code>EclipticPrecessor</code>](#module_precess.EclipticPrecessor)  
**Returns**: <code>elementequinox.Elements</code> - eTo  

| Param | Type |
| --- | --- |
| eFrom | <code>elementequinox.Elements</code> | 

<a name="module_precess.approxAnnualPrecession"></a>

### precess.approxAnnualPrecession(eqFrom, epochFrom, epochTo) ⇒ <code>Array</code>
approxAnnualPrecession returns approximate annual precision in right
ascension and declination.

The two epochs should be within a few hundred years.
The declinations should not be too close to the poles.

**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>Array</code> - {sexa.HourAngle} seconds of right ascension
 {sexa.Angle} seconds of Declination  

| Param | Type | Description |
| --- | --- | --- |
| eqFrom | <code>coord.Equatorial</code> |  |
| epochFrom | <code>Number</code> | use `base.JDEToJulianYear(year)` to get epoch |
| epochTo | <code>Number</code> | use `base.JDEToJulianYear(year)` to get epoch |

<a name="module_precess.mn"></a>

### precess.mn(epochFrom, epochTo)
**Kind**: static method of [<code>precess</code>](#module_precess)  

| Param | Type | Description |
| --- | --- | --- |
| epochFrom | <code>Number</code> | use `base.JDEToJulianYear(year)` to get epoch |
| epochTo | <code>Number</code> | use `base.JDEToJulianYear(year)` to get epoch |

<a name="module_precess.approxPosition"></a>

### precess.approxPosition(eqFrom, epochFrom, epochTo, mα, mδ) ⇒ <code>coord.Equatorial</code>
ApproxPosition uses ApproxAnnualPrecession to compute a simple and quick
precession while still considering proper motion.

**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>coord.Equatorial</code> - eqTo  

| Param | Type | Description |
| --- | --- | --- |
| eqFrom | <code>coord.Equatorial</code> |  |
| epochFrom | <code>Number</code> |  |
| epochTo | <code>Number</code> |  |
| mα | <code>Number</code> | in radians |
| mδ | <code>Number</code> | in radians |

<a name="module_precess.position"></a>

### precess.position(eqFrom, eqTo, epochFrom, epochTo, mα, mδ) ⇒ <code>coord.Equatorial</code>
Position precesses equatorial coordinates from one epoch to another,
including proper motions.

If proper motions are not to be considered or are not applicable, pass 0, 0
for mα, mδ

Both eqFrom and eqTo must be non-nil, although they may point to the same
struct.  EqTo is returned for convenience.

**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>coord.Equatorial</code> - [eqTo]  

| Param | Type | Description |
| --- | --- | --- |
| eqFrom | <code>coord.Equatorial</code> |  |
| eqTo | <code>coord.Equatorial</code> |  |
| epochFrom | <code>Number</code> |  |
| epochTo | <code>Number</code> |  |
| mα | <code>Number</code> | in radians |
| mδ | <code>Number</code> | in radians |

<a name="module_precess.eclipticPosition"></a>

### precess.eclipticPosition(eclFrom,, epochFrom, epochTo, mα, mδ) ⇒ <code>coord.Ecliptic</code>
eclipticPosition precesses ecliptic coordinates from one epoch to another,
including proper motions.
While eclFrom is given as ecliptic coordinates, proper motions mα, mδ are
still expected to be equatorial.  If proper motions are not to be considered
or are not applicable, pass 0, 0.
Both eclFrom and eclTo must be non-nil, although they may point to the same
struct.  EclTo is returned for convenience.

**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>coord.Ecliptic</code> - eclTo  

| Param | Type |
| --- | --- |
| eclFrom, | <code>coord.Ecliptic</code> | 
| epochFrom | <code>Number</code> | 
| epochTo | <code>Number</code> | 
| mα | <code>sexa.HourAngle</code> | 
| mδ | <code>sexa.Angle</code> | 

<a name="module_precess.properMotion"></a>

### precess.properMotion(mα, mδ, epoch, ecl) ⇒ <code>Array.&lt;Number&gt;</code>
**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>Array.&lt;Number&gt;</code> - [mλ, mβ]  

| Param | Type | Description |
| --- | --- | --- |
| mα | <code>Number</code> | anual proper motion (ra) |
| mδ | <code>Number</code> | anual proper motion (dec) |
| epoch | <code>Number</code> |  |
| ecl | <code>coord.Ecliptic</code> |  |

<a name="module_precess.properMotion3D"></a>

### precess.properMotion3D(eqFrom,, epochFrom, r, mr, mα, mδ) ⇒ <code>coord.Equatorial</code>
ProperMotion3D takes the 3D equatorial coordinates of an object
at one epoch and computes its coordinates at a new epoch, considering
proper motion and radial velocity.

Radial distance (r) must be in parsecs, radial velocitiy (mr) in
parsecs per year.

Both eqFrom and eqTo must be non-nil, although they may point to the same
struct.  EqTo is returned for convenience.

**Kind**: static method of [<code>precess</code>](#module_precess)  
**Returns**: <code>coord.Equatorial</code> - eqTo  

| Param | Type |
| --- | --- |
| eqFrom, | <code>coord.Equatorial</code> | 
| epochFrom | <code>Number</code> | 
| r | <code>Number</code> | 
| mr | <code>Number</code> | 
| mα | <code>sexa.HourAngle</code> | 
| mδ | <code>sexa.Angle</code> | 

<a name="module_refraction"></a>

## refraction
**License**: MIT  
**Copyright**: 2016 commenthol  

* [refraction](#module_refraction)
    * [.gt15True()](#module_refraction.gt15True)
    * [.gt15Apparent()](#module_refraction.gt15Apparent)
    * [.bennett()](#module_refraction.bennett)
    * [.bennett2()](#module_refraction.bennett2)
    * [.saemundsson()](#module_refraction.saemundsson)

<a name="module_refraction.gt15True"></a>

### refraction.gt15True()
gt15True returns refraction for obtaining true altitude when altitude
is greater than 15 degrees (about 0.26 radians.)

h0 must be a measured apparent altitude of a celestial body in radians.

Result is refraction to be subtracted from h0 to obtain the true altitude
of the body.  Unit is radians.

**Kind**: static method of [<code>refraction</code>](#module_refraction)  
<a name="module_refraction.gt15Apparent"></a>

### refraction.gt15Apparent()
gt15Apparent returns refraction for obtaining apparent altitude when
altitude is greater than 15 degrees (about 0.26 radians.)

h must be a computed true "airless" altitude of a celestial body in radians.

Result is refraction to be added to h to obtain the apparent altitude
of the body.  Unit is radians.

**Kind**: static method of [<code>refraction</code>](#module_refraction)  
<a name="module_refraction.bennett"></a>

### refraction.bennett()
Bennett returns refraction for obtaining true altitude.

h0 must be a measured apparent altitude of a celestial body in radians.

Results are accurate to 0.07 arc min from horizon to zenith.

Result is refraction to be subtracted from h0 to obtain the true altitude
of the body.  Unit is radians.

**Kind**: static method of [<code>refraction</code>](#module_refraction)  
<a name="module_refraction.bennett2"></a>

### refraction.bennett2()
Bennett2 returns refraction for obtaining true altitude.

Similar to Bennett, but a correction is applied to give a more accurate
result.

Results are accurate to 0.015 arc min.  Result unit is radians.

**Kind**: static method of [<code>refraction</code>](#module_refraction)  
<a name="module_refraction.saemundsson"></a>

### refraction.saemundsson()
Saemundsson returns refraction for obtaining apparent altitude.

h must be a computed true "airless" altitude of a celestial body in radians.

Result is refraction to be added to h to obtain the apparent altitude
of the body.

Results are consistent with Bennett to within 4 arc sec.
Result unit is radians.

**Kind**: static method of [<code>refraction</code>](#module_refraction)  
<a name="module_rise"></a>

## rise
**License**: MIT  
**Copyright**: 2016 commenthol  

* [rise](#module_rise)
    * _static_
        * [.PlanetRise](#module_rise.PlanetRise)
            * [new exports.PlanetRise(jd, lat, lon, earth, planet, opts)](#new_module_rise.PlanetRise_new)
        * [.meanRefraction](#module_rise.meanRefraction)
        * [.stdh0](#module_rise.stdh0)
        * [.stdh0Stellar](#module_rise.stdh0Stellar)
        * [.stdh0Solar](#module_rise.stdh0Solar)
        * [.stdh0LunarMean](#module_rise.stdh0LunarMean)
        * [.stdh0Lunar](#module_rise.stdh0Lunar) ⇒ <code>number</code>
        * [.refraction(h0, corr)](#module_rise.refraction) ⇒ <code>number</code>
        * [.hourAngle()](#module_rise.hourAngle) ⇒ <code>number</code>
        * [.approxTimes(p, h0, Th0, α3, δ3)](#module_rise.approxTimes) ⇒
        * [.times(p, ΔT, h0, Th0, α3, δ3)](#module_rise.times) ⇒
    * _inner_
        * [~_mt(lon, α, th0)](#module_rise.._mt) ⇒ <code>number</code>
        * [~_th0(Th0, m)](#module_rise.._th0) ⇒ <code>number</code>

<a name="module_rise.PlanetRise"></a>

### rise.PlanetRise
RisePlanet computes rise, transit and set times for a planet on a day of interest.

**Kind**: static class of [<code>rise</code>](#module_rise)  
<a name="new_module_rise.PlanetRise_new"></a>

#### new exports.PlanetRise(jd, lat, lon, earth, planet, opts)

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> \| <code>Date</code> | Julian Day starting at midnight or Date object |
| lat | <code>number</code> | geographic latitude of the observerin degrees |
| lon | <code>number</code> | geographic longitude of the observer in degrees (measured positively westward) |
| earth | <code>planetposition.Planet</code> | VSOP87 Planet object for Earth |
| planet | <code>planetposition.Planet</code> | VSOP87 Planet object of observed body |
| opts | <code>object</code> |  |
| opts.date | <code>boolean</code> | return times as Date objects |
| opts.refraction | <code>number</code> | use different refraction than `stdh0Stellar` |

<a name="module_rise.meanRefraction"></a>

### rise.meanRefraction
mean refraction of the atmosphere

**Kind**: static constant of [<code>rise</code>](#module_rise)  
<a name="module_rise.stdh0"></a>

### rise.stdh0
"Standard altitudes" for various bodies already including `meanRefraction` of 0°34'

The standard altitude is the geometric altitude of the center of body
at the time of apparent rising or seting.

**Kind**: static constant of [<code>rise</code>](#module_rise)  
<a name="module_rise.stdh0Stellar"></a>

### rise.stdh0Stellar
standard altitude for stars, planets at apparent rising, seting

**Kind**: static constant of [<code>rise</code>](#module_rise)  
<a name="module_rise.stdh0Solar"></a>

### rise.stdh0Solar
standard altitude for sun for upper limb of the disk

**Kind**: static constant of [<code>rise</code>](#module_rise)  
<a name="module_rise.stdh0LunarMean"></a>

### rise.stdh0LunarMean
standard altitude for moon (low accuracy)

**Kind**: static constant of [<code>rise</code>](#module_rise)  
<a name="module_rise.stdh0Lunar"></a>

### rise.stdh0Lunar ⇒ <code>number</code>
Stdh0Lunar is the standard altitude of the Moon considering π, the
Moon's horizontal parallax.

**Kind**: static constant of [<code>rise</code>](#module_rise)  
**Returns**: <code>number</code> - altitude of Moon in radians  

| Param | Type | Description |
| --- | --- | --- |
| π | <code>number</code> | the Moon's horizontal parallax |
| [refraction] | <code>number</code> | optional value for refraction in radians if        omitted than meanRefraction is used |

<a name="module_rise.refraction"></a>

### rise.refraction(h0, corr) ⇒ <code>number</code>
Helper function to obtain corrected refraction

**Kind**: static method of [<code>rise</code>](#module_rise)  
**Returns**: <code>number</code> - refraction value in radians  

| Param | Type | Description |
| --- | --- | --- |
| h0 | <code>number</code> | altitude of the body in radians containing `meanRefraction` of 0°34' |
| corr | <code>number</code> | the calcluated refraction e.g. from package `refraction` in radians |

<a name="module_rise.hourAngle"></a>

### rise.hourAngle() ⇒ <code>number</code>
**Kind**: static method of [<code>rise</code>](#module_rise)  
**Returns**: <code>number</code> - local angle in radians  
<a name="module_rise.approxTimes"></a>

### rise.approxTimes(p, h0, Th0, α3, δ3) ⇒
ApproxTimes computes approximate UT rise, transit and set times for
a celestial object on a day of interest.

The function argurments do not actually include the day, but do include
values computed from the day.

**Kind**: static method of [<code>rise</code>](#module_rise)  
**Returns**: Result units are seconds and are in the range [0,86400)  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| p | <code>coord.Globe</code> | is geographic coordinates of observer. |
| h0 | <code>number</code> | is "standard altitude" of the body in radians |
| Th0 | <code>number</code> | is apparent sidereal time at 0h UT at Greenwich in seconds        (range 0...86400) must be the time on the day of interest, in seconds.        See sidereal.apparent0UT |
| α3 | <code>Array.&lt;number&gt;</code> | slices of three right ascensions |
| δ3 | <code>Array.&lt;number&gt;</code> | slices of three declinations.        α3, δ3 must be values at 0h dynamical time for the day before, the day of,        and the day after the day of interest.  Units are radians. |

<a name="module_rise.times"></a>

### rise.times(p, ΔT, h0, Th0, α3, δ3) ⇒
Times computes UT rise, transit and set times for a celestial object on
a day of interest.

The function argurments do not actually include the day, but do include
a number of values computed from the day.

**Kind**: static method of [<code>rise</code>](#module_rise)  
**Returns**: Result units are seconds and are in the range [0,86400)  
**Throws**:

- Error


| Param | Type | Description |
| --- | --- | --- |
| p | <code>coord.Globe</code> | is geographic coordinates of observer. |
| ΔT | <code>number</code> | is delta T in seconds |
| h0 | <code>number</code> | is "standard altitude" of the body in radians |
| Th0 | <code>number</code> | is apparent sidereal time at 0h UT at Greenwich in seconds        (range 0...86400) must be the time on the day of interest, in seconds.        See sidereal.apparent0UT |
| α3 | <code>Array.&lt;number&gt;</code> | slices of three right ascensions |
| δ3 | <code>Array.&lt;number&gt;</code> | slices of three declinations.        α3, δ3 must be values at 0h dynamical time for the day before, the day of,        and the day after the day of interest.  Units are radians. |

<a name="module_rise.._mt"></a>

### rise~\_mt(lon, α, th0) ⇒ <code>number</code>
**Kind**: inner method of [<code>rise</code>](#module_rise)  
**Returns**: <code>number</code> - time of transit in seconds of day `[0, 86400[`  

| Param | Type | Description |
| --- | --- | --- |
| lon | <code>number</code> | longitude in radians |
| α | <code>number</code> | right ascension in radians |
| th0 | <code>number</code> | sidereal.apparent0UT in seconds of day `[0...86400[` |

<a name="module_rise.._th0"></a>

### rise~\_th0(Th0, m) ⇒ <code>number</code>
**Kind**: inner method of [<code>rise</code>](#module_rise)  
**Returns**: <code>number</code> - new siderial time seconds of day `[0...86400[`  

| Param | Type | Description |
| --- | --- | --- |
| Th0 | <code>number</code> | sidereal.apparent0UT in seconds of day `[0...86400[` |
| m | <code>number</code> | motion in seconds of day `[0...86400[` |

<a name="module_saturnmoons"></a>

## saturnmoons
**License**: MIT  
**Copyright**: 2016 commenthol  

* [saturnmoons](#module_saturnmoons)
    * _static_
        * [.positions(jde, earth, saturn)](#module_saturnmoons.positions) ⇒ <code>Array.&lt;XY&gt;</code>
    * _inner_
        * [~XY()](#module_saturnmoons..XY)

<a name="module_saturnmoons.positions"></a>

### saturnmoons.positions(jde, earth, saturn) ⇒ <code>Array.&lt;XY&gt;</code>
Positions returns positions of the eight major moons of Saturn.

Results returned in argument pos, which must not be undefined.

Result units are Saturn radii.

**Kind**: static method of [<code>saturnmoons</code>](#module_saturnmoons)  
**Returns**: <code>Array.&lt;XY&gt;</code> - Array of Moon Positions in `XY`
  Use `M.mimas ... M.iapetus` to resolve to Moon and its position at `jde`  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>number</code> | Julian ephemeris day |
| earth | <code>planetposition.Planet</code> | VSOP87 planet Earth |
| saturn | <code>planetposition.Planet</code> | VSOP87 planet Saturn |

<a name="module_saturnmoons..XY"></a>

### saturnmoons~XY()
XY holds coordinates returned from positions().

**Kind**: inner method of [<code>saturnmoons</code>](#module_saturnmoons)  
<a name="module_saturnring"></a>

## saturnring
**License**: MIT  
**Copyright**: 2016 commenthol  

* [saturnring](#module_saturnring)
    * _static_
        * [.ring()](#module_saturnring.ring)
        * [.ub()](#module_saturnring.ub)
    * _inner_
        * [~cl()](#module_saturnring..cl)

<a name="module_saturnring.ring"></a>

### saturnring.ring()
Ring computes quantities of the ring of Saturn.

 B  Saturnicentric latitude of the Earth referred to the plane of the ring.
 Bʹ  Saturnicentric latitude of the Sun referred to the plane of the ring.
 ΔU  Difference between Saturnicentric longitudes of the Sun and the Earth.
 P  Geometric position angle of the northern semiminor axis of the ring.
 aEdge  Major axis of the out edge of the outer ring.
 bEdge  Minor axis of the out edge of the outer ring.

All results in radians.

**Kind**: static method of [<code>saturnring</code>](#module_saturnring)  
<a name="module_saturnring.ub"></a>

### saturnring.ub()
UB computes quantities required by illum.Saturn().

Same as ΔU and B returned by Ring().  Results in radians.

**Kind**: static method of [<code>saturnring</code>](#module_saturnring)  
<a name="module_saturnring..cl"></a>

### saturnring~cl()
cl splits the work into two closures.

**Kind**: inner method of [<code>saturnring</code>](#module_saturnring)  
<a name="module_semidiameter"></a>

## semidiameter
**License**: MIT  
**Copyright**: 2016 commenthol  

* [semidiameter](#module_semidiameter)
    * [.Sun](#module_semidiameter.Sun)
    * [.semidiameter()](#module_semidiameter.semidiameter)
    * [.aaturnApparentPolar()](#module_semidiameter.aaturnApparentPolar)
    * [.moonTopocentric()](#module_semidiameter.moonTopocentric)
    * [.moonTopocentric2()](#module_semidiameter.moonTopocentric2)
    * [.asteroidDiameter()](#module_semidiameter.asteroidDiameter)
    * [.asteroid()](#module_semidiameter.asteroid)

<a name="module_semidiameter.Sun"></a>

### semidiameter.Sun
Standard semidiameters at unit distance of 1 AU.
Values are scaled here to radians.

**Kind**: static constant of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.semidiameter"></a>

### semidiameter.semidiameter()
Semidiameter returns semidiameter at specified distance.

When used with S0 values provided, Δ must be observer-body distance in AU.
Result will then be in radians.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.aaturnApparentPolar"></a>

### semidiameter.aaturnApparentPolar()
SaturnApparentPolar returns apparent polar semidiameter of Saturn
at specified distance.

Argument Δ must be observer-Saturn distance in AU.  Argument B is
Saturnicentric latitude of the observer as given by function saturnring.UB()
for example.

Result is semidiameter in units of package variables SaturnPolar and
SaturnEquatorial, nominally radians.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.moonTopocentric"></a>

### semidiameter.moonTopocentric()
MoonTopocentric returns observed topocentric semidiameter of the Moon.

 Δ is distance to Moon in AU.
 δ is declination of Moon in radians.
 H is hour angle of Moon in radians.
 ρsφʹ, ρcφʹ are parallax constants as returned by
     globe.Ellipsoid.ParallaxConstants, for example.

Result is semidiameter in radians.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.moonTopocentric2"></a>

### semidiameter.moonTopocentric2()
MoonTopocentric2 returns observed topocentric semidiameter of the Moon
by a less rigorous method.

Δ is distance to Moon in AU, h is altitude of the Moon above the observer's
horizon in radians.

Result is semidiameter in radians.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.asteroidDiameter"></a>

### semidiameter.asteroidDiameter()
AsteroidDiameter returns approximate diameter given absolute magnitude H
and albedo A.

Result is in km.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_semidiameter.asteroid"></a>

### semidiameter.asteroid()
Asteroid returns semidiameter of an asteroid with a given diameter
at given distance.

Argument d is diameter in km, Δ is distance in AU.

Result is semidiameter in radians.

**Kind**: static method of [<code>semidiameter</code>](#module_semidiameter)  
<a name="module_sexagesimal"></a>

## sexagesimal
**License**: MIT  
**Copyright**: 2016 commenthol  

* [sexagesimal](#module_sexagesimal)
    * [.Angle](#module_sexagesimal.Angle)
        * [new exports.Angle(angle, neg, d, m, s)](#new_module_sexagesimal.Angle_new)
        * [.setDMS(neg, d, m, s)](#module_sexagesimal.Angle+setDMS) ⇒ <code>Angle</code>
        * [.setAngle(angle)](#module_sexagesimal.Angle+setAngle) ⇒ <code>Angle</code>
        * [.rad()](#module_sexagesimal.Angle+rad) ⇒ <code>Number</code>
        * [.deg()](#module_sexagesimal.Angle+deg) ⇒ <code>Number</code>
        * [.toDMS()](#module_sexagesimal.Angle+toDMS)
        * [.toString(precision)](#module_sexagesimal.Angle+toString) ⇒ <code>String</code>
        * [.toDegString(precision)](#module_sexagesimal.Angle+toDegString) ⇒ <code>String</code>
    * [.HourAngle](#module_sexagesimal.HourAngle)
        * [.setDMS(neg, h, m, s)](#module_sexagesimal.HourAngle+setDMS) ⇒ <code>Angle</code>
        * [.hour()](#module_sexagesimal.HourAngle+hour) ⇒
        * [.toString(precision)](#module_sexagesimal.HourAngle+toString) ⇒ <code>String</code>
    * [.RA](#module_sexagesimal.RA)
        * [new exports.RA(h, m, s)](#new_module_sexagesimal.RA_new)
    * [.Time](#module_sexagesimal.Time)
        * [new exports.Time(neg, h, m, s)](#new_module_sexagesimal.Time_new)
        * [.sec()](#module_sexagesimal.Time+sec) ⇒ <code>Number</code>
        * [.min()](#module_sexagesimal.Time+min) ⇒ <code>Number</code>
        * [.hour()](#module_sexagesimal.Time+hour) ⇒ <code>Number</code>
        * [.day()](#module_sexagesimal.Time+day) ⇒ <code>Number</code>
        * [.rad()](#module_sexagesimal.Time+rad) ⇒ <code>Number</code>
        * [.toHMS()](#module_sexagesimal.Time+toHMS) ⇒ <code>Array</code>
        * [.toString(precision)](#module_sexagesimal.Time+toString) ⇒ <code>String</code>
    * [.DMSToDeg(neg, d, m, s)](#module_sexagesimal.DMSToDeg) ⇒ <code>Number</code>
    * [.degToDMS(deg)](#module_sexagesimal.degToDMS) ⇒ <code>Array</code>

<a name="module_sexagesimal.Angle"></a>

### sexagesimal.Angle
Angle represents a general purpose angle.
Unit is radians.

**Kind**: static class of [<code>sexagesimal</code>](#module_sexagesimal)  

* [.Angle](#module_sexagesimal.Angle)
    * [new exports.Angle(angle, neg, d, m, s)](#new_module_sexagesimal.Angle_new)
    * [.setDMS(neg, d, m, s)](#module_sexagesimal.Angle+setDMS) ⇒ <code>Angle</code>
    * [.setAngle(angle)](#module_sexagesimal.Angle+setAngle) ⇒ <code>Angle</code>
    * [.rad()](#module_sexagesimal.Angle+rad) ⇒ <code>Number</code>
    * [.deg()](#module_sexagesimal.Angle+deg) ⇒ <code>Number</code>
    * [.toDMS()](#module_sexagesimal.Angle+toDMS)
    * [.toString(precision)](#module_sexagesimal.Angle+toString) ⇒ <code>String</code>
    * [.toDegString(precision)](#module_sexagesimal.Angle+toDegString) ⇒ <code>String</code>

<a name="new_module_sexagesimal.Angle_new"></a>

#### new exports.Angle(angle, neg, d, m, s)
constructs a new Angle value from sign, degree, minute, and second
components.
__One argument__


| Param | Type | Description |
| --- | --- | --- |
| angle | <code>Number</code> | (float) angle in radians __Four arguments__ |
| neg | <code>Boolean</code> | sign, true if negative (required to attribute -0°30') |
| d | <code>Number</code> | (int) degree |
| m | <code>Number</code> | (int) minute |
| s | <code>Number</code> | (float) second |

<a name="module_sexagesimal.Angle+setDMS"></a>

#### angle.setDMS(neg, d, m, s) ⇒ <code>Angle</code>
SetDMS sets the value of an FAngle from sign, degree, minute, and second
components.
The receiver is returned as a convenience.

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| neg | <code>Boolean</code> | <code>0</code> | sign, true if negative |
| d | <code>Number</code> | <code>0</code> | (int) degree |
| m | <code>Number</code> | <code>0</code> | (int) minute |
| s | <code>Number</code> | <code>0</code> | (float) second |

<a name="module_sexagesimal.Angle+setAngle"></a>

#### angle.setAngle(angle) ⇒ <code>Angle</code>
sets angle

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  

| Param | Type | Description |
| --- | --- | --- |
| angle | <code>Number</code> | (float) angle in radians |

<a name="module_sexagesimal.Angle+rad"></a>

#### angle.rad() ⇒ <code>Number</code>
Rad returns the angle in radians.

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  
**Returns**: <code>Number</code> - angle in radians  
<a name="module_sexagesimal.Angle+deg"></a>

#### angle.deg() ⇒ <code>Number</code>
Deg returns the angle in degrees.

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  
**Returns**: <code>Number</code> - angle in degree  
<a name="module_sexagesimal.Angle+toDMS"></a>

#### angle.toDMS()
toDMS converts to parsed sexagesimal angle component.

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  
<a name="module_sexagesimal.Angle+toString"></a>

#### angle.toString(precision) ⇒ <code>String</code>
Print angle in degree using `d°m´s.ss″`

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  

| Param | Type | Description |
| --- | --- | --- |
| precision | <code>Number</code> | precision of `s.ss` |

<a name="module_sexagesimal.Angle+toDegString"></a>

#### angle.toDegString(precision) ⇒ <code>String</code>
Print angle in degree using `d°.ff`

**Kind**: instance method of [<code>Angle</code>](#module_sexagesimal.Angle)  

| Param | Type | Description |
| --- | --- | --- |
| precision | <code>Number</code> | precision of `.ff` |

<a name="module_sexagesimal.HourAngle"></a>

### sexagesimal.HourAngle
HourAngle represents an angle corresponding to angular rotation of
the Earth in a specified time.

Unit is radians.

**Kind**: static class of [<code>sexagesimal</code>](#module_sexagesimal)  

* [.HourAngle](#module_sexagesimal.HourAngle)
    * [.setDMS(neg, h, m, s)](#module_sexagesimal.HourAngle+setDMS) ⇒ <code>Angle</code>
    * [.hour()](#module_sexagesimal.HourAngle+hour) ⇒
    * [.toString(precision)](#module_sexagesimal.HourAngle+toString) ⇒ <code>String</code>

<a name="module_sexagesimal.HourAngle+setDMS"></a>

#### hourAngle.setDMS(neg, h, m, s) ⇒ <code>Angle</code>
SetDMS sets the value of an FAngle from sign, degree, minute, and second
components.
The receiver is returned as a convenience.

**Kind**: instance method of [<code>HourAngle</code>](#module_sexagesimal.HourAngle)  

| Param | Type | Default | Description |
| --- | --- | --- | --- |
| neg | <code>Boolean</code> | <code>0</code> | sign, true if negative |
| h | <code>Number</code> | <code>0</code> | (int) hour |
| m | <code>Number</code> | <code>0</code> | (int) minute |
| s | <code>Number</code> | <code>0</code> | (float) second |

<a name="module_sexagesimal.HourAngle+hour"></a>

#### hourAngle.hour() ⇒
Hour returns the hour angle as hours of time.

**Kind**: instance method of [<code>HourAngle</code>](#module_sexagesimal.HourAngle)  
**Returns**: hour angle  
<a name="module_sexagesimal.HourAngle+toString"></a>

#### hourAngle.toString(precision) ⇒ <code>String</code>
Print angle in `HʰMᵐs.ssˢ`

**Kind**: instance method of [<code>HourAngle</code>](#module_sexagesimal.HourAngle)  

| Param | Type | Description |
| --- | --- | --- |
| precision | <code>Number</code> | precision of `s.ss` |

<a name="module_sexagesimal.RA"></a>

### sexagesimal.RA
TODO

**Kind**: static class of [<code>sexagesimal</code>](#module_sexagesimal)  
<a name="new_module_sexagesimal.RA_new"></a>

#### new exports.RA(h, m, s)
constructs a new RA value from hour, minute, and second components.
Negative values are not supported, RA wraps values larger than 24
to the range [0,24) hours.


| Param | Type | Default | Description |
| --- | --- | --- | --- |
| h | <code>Number</code> | <code>0</code> | (int) hour |
| m | <code>Number</code> | <code>0</code> | (int) minute |
| s | <code>Number</code> | <code>0</code> | (float) second |

<a name="module_sexagesimal.Time"></a>

### sexagesimal.Time
Time Angle
Unit is time in seconds.

**Kind**: static class of [<code>sexagesimal</code>](#module_sexagesimal)  

* [.Time](#module_sexagesimal.Time)
    * [new exports.Time(neg, h, m, s)](#new_module_sexagesimal.Time_new)
    * [.sec()](#module_sexagesimal.Time+sec) ⇒ <code>Number</code>
    * [.min()](#module_sexagesimal.Time+min) ⇒ <code>Number</code>
    * [.hour()](#module_sexagesimal.Time+hour) ⇒ <code>Number</code>
    * [.day()](#module_sexagesimal.Time+day) ⇒ <code>Number</code>
    * [.rad()](#module_sexagesimal.Time+rad) ⇒ <code>Number</code>
    * [.toHMS()](#module_sexagesimal.Time+toHMS) ⇒ <code>Array</code>
    * [.toString(precision)](#module_sexagesimal.Time+toString) ⇒ <code>String</code>

<a name="new_module_sexagesimal.Time_new"></a>

#### new exports.Time(neg, h, m, s)

| Param | Type | Description |
| --- | --- | --- |
| neg | <code>Boolean</code> | set `true` if negative |
| h | <code>Number</code> | (int) hour |
| m | <code>Number</code> | (int) minute |
| s | <code>Number</code> | (float) second |

<a name="module_sexagesimal.Time+sec"></a>

#### time.sec() ⇒ <code>Number</code>
**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Number</code> - time in seconds.  
<a name="module_sexagesimal.Time+min"></a>

#### time.min() ⇒ <code>Number</code>
**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Number</code> - time in minutes.  
<a name="module_sexagesimal.Time+hour"></a>

#### time.hour() ⇒ <code>Number</code>
**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Number</code> - time in hours.  
<a name="module_sexagesimal.Time+day"></a>

#### time.day() ⇒ <code>Number</code>
**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Number</code> - time in days.  
<a name="module_sexagesimal.Time+rad"></a>

#### time.rad() ⇒ <code>Number</code>
**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Number</code> - time in radians, where 1 day = 2 Pi radians.  
<a name="module_sexagesimal.Time+toHMS"></a>

#### time.toHMS() ⇒ <code>Array</code>
convert time to HMS

**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  
**Returns**: <code>Array</code> - [neg, h, m, s]
 {Boolean} neg - sign, true if negative
 {Number} h - (int) hour
 {Number} m - (int) minute
 {Number} s - (float) second  
<a name="module_sexagesimal.Time+toString"></a>

#### time.toString(precision) ⇒ <code>String</code>
Print time using `HʰMᵐsˢ.ss`

**Kind**: instance method of [<code>Time</code>](#module_sexagesimal.Time)  

| Param | Type | Description |
| --- | --- | --- |
| precision | <code>Number</code> | precision of `.ss` |

<a name="module_sexagesimal.DMSToDeg"></a>

### sexagesimal.DMSToDeg(neg, d, m, s) ⇒ <code>Number</code>
DMSToDeg converts from parsed sexagesimal angle components to decimal
degrees.

**Kind**: static method of [<code>sexagesimal</code>](#module_sexagesimal)  
**Returns**: <code>Number</code> - angle in degree  

| Param | Type | Description |
| --- | --- | --- |
| neg | <code>Boolean</code> | sign, true if negative |
| d | <code>Number</code> | (int) degree |
| m | <code>Number</code> | (int) minute |
| s | <code>Number</code> | (float) second |

<a name="module_sexagesimal.degToDMS"></a>

### sexagesimal.degToDMS(deg) ⇒ <code>Array</code>
DegToDMS converts from decimal degrees to parsed sexagesimal angle component.

**Kind**: static method of [<code>sexagesimal</code>](#module_sexagesimal)  
**Returns**: <code>Array</code> - [neg, d, m, s]
 {Boolean} neg - sign, true if negative
 {Number} d - (int) degree
 {Number} m - (int) minute
 {Number} s - (float) second  

| Param | Type | Description |
| --- | --- | --- |
| deg | <code>Number</code> | angle in degree |

<a name="module_sidereal"></a>

## sidereal
**License**: MIT  
**Copyright**: 2016 commenthol  

* [sidereal](#module_sidereal)
    * [.iau82](#module_sidereal.iau82)
    * [.JDToCFrac(jd)](#module_sidereal.JDToCFrac) ⇒ <code>Array.&lt;number&gt;</code>
    * [.mean(jd)](#module_sidereal.mean) ⇒ <code>number</code>
    * [.mean0UT(jd)](#module_sidereal.mean0UT) ⇒ <code>number</code>
    * [.apparent(jd)](#module_sidereal.apparent) ⇒ <code>number</code>
    * [.apparent0UT(jd)](#module_sidereal.apparent0UT) ⇒ <code>number</code>

<a name="module_sidereal.iau82"></a>

### sidereal.iau82
iau82 is a polynomial giving mean sidereal time at Greenwich at 0h UT.

The polynomial is in centuries from J2000.0, as given by JDToCFrac.
Coefficients are those adopted in 1982 by the International Astronomical
Union and are given in (12.2) p. 87.

**Kind**: static constant of [<code>sidereal</code>](#module_sidereal)  
<a name="module_sidereal.JDToCFrac"></a>

### sidereal.JDToCFrac(jd) ⇒ <code>Array.&lt;number&gt;</code>
JDToCFrac returns values for use in computing sidereal time at Greenwich.

Cen is centuries from J2000 of the JD at 0h UT of argument jd.  This is
the value to use for evaluating the IAU sidereal time polynomial.
DayFrac is the fraction of jd after 0h UT.  It is used to compute the
final value of sidereal time.

**Kind**: static method of [<code>sidereal</code>](#module_sidereal)  
**Returns**: <code>Array.&lt;number&gt;</code> - [century, fraction] century and fraction of jd after 0h UT  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian Days |

<a name="module_sidereal.mean"></a>

### sidereal.mean(jd) ⇒ <code>number</code>
Mean returns mean sidereal time at Greenwich for a given JD.

Computation is by IAU 1982 coefficients.  The result is in seconds of
time and is in the range [0,86400).

**Kind**: static method of [<code>sidereal</code>](#module_sidereal)  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian Days |

<a name="module_sidereal.mean0UT"></a>

### sidereal.mean0UT(jd) ⇒ <code>number</code>
Mean0UT returns mean sidereal time at Greenwich at 0h UT on the given JD.

The result is in seconds of time and is in the range [0,86400).

**Kind**: static method of [<code>sidereal</code>](#module_sidereal)  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian Days |

<a name="module_sidereal.apparent"></a>

### sidereal.apparent(jd) ⇒ <code>number</code>
Apparent returns apparent sidereal time at Greenwich for the given JD.

Apparent is mean plus the nutation in right ascension.

The result is in seconds of time and is in the range [0,86400).

**Kind**: static method of [<code>sidereal</code>](#module_sidereal)  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian Days |

<a name="module_sidereal.apparent0UT"></a>

### sidereal.apparent0UT(jd) ⇒ <code>number</code>
Apparent0UT returns apparent sidereal time at Greenwich at 0h UT
on the given JD.

The result is in seconds of time and is in the range [0,86400).

**Kind**: static method of [<code>sidereal</code>](#module_sidereal)  

| Param | Type | Description |
| --- | --- | --- |
| jd | <code>number</code> | Julian Days |

<a name="module_solar"></a>

## solar
**License**: MIT  
**Copyright**: 2016 commenthol  

* [solar](#module_solar)
    * [.trueLongitude(T)](#module_solar.trueLongitude) ⇒ <code>Object</code>
    * [.meanAnomaly(T)](#module_solar.meanAnomaly) ⇒ <code>Number</code>
    * [.eccentricity(T)](#module_solar.eccentricity) ⇒ <code>Number</code>
    * [.radius(T)](#module_solar.radius) ⇒ <code>Number</code>
    * [.apparentLongitude(T)](#module_solar.apparentLongitude) ⇒ <code>Number</code>
    * [.true2000(T)](#module_solar.true2000) ⇒ <code>Object</code>
    * [.trueEquatorial(jde)](#module_solar.trueEquatorial) ⇒ <code>base.Coord</code>
    * [.apparentEquatorial(jde)](#module_solar.apparentEquatorial) ⇒ <code>base.Coord</code>
    * [.trueVSOP87(planet, jde)](#module_solar.trueVSOP87) ⇒ <code>Object</code>
    * [.apparentVSOP87(planet, jde)](#module_solar.apparentVSOP87) ⇒ <code>base.Coord</code>
    * [.apparentEquatorialVSOP87(planet, jde)](#module_solar.apparentEquatorialVSOP87) ⇒ <code>Number</code>
    * [.aberration(range)](#module_solar.aberration) ⇒ <code>Number</code>

<a name="module_solar.trueLongitude"></a>

### solar.trueLongitude(T) ⇒ <code>Object</code>
True returns true geometric longitude and anomaly of the sun referenced to the mean equinox of date.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Object</code> - {Number} lon = true geometric longitude, ☉, in radians
  {Number} ano = true anomaly in radians  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.meanAnomaly"></a>

### solar.meanAnomaly(T) ⇒ <code>Number</code>
meanAnomaly returns the mean anomaly of Earth at the given T.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - Result is in radians and is not normalized to the range 0..2π.  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.eccentricity"></a>

### solar.eccentricity(T) ⇒ <code>Number</code>
eccentricity returns eccentricity of the Earth's orbit around the sun.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - eccentricity of the Earth's orbit around the sun.  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.radius"></a>

### solar.radius(T) ⇒ <code>Number</code>
Radius returns the Sun-Earth distance in AU.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - Sun-Earth distance in AU  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.apparentLongitude"></a>

### solar.apparentLongitude(T) ⇒ <code>Number</code>
ApparentLongitude returns apparent longitude of the Sun referenced to the true equinox of date.
Result includes correction for nutation and aberration.  Unit is radians.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - apparent longitude of the Sun referenced to the true equinox of date.  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.true2000"></a>

### solar.true2000(T) ⇒ <code>Object</code>
true2000 returns true geometric longitude and anomaly of the sun referenced to equinox J2000.
Results are accurate to .01 degree for years 1900 to 2100.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Object</code> - {Number} lon - true geometric longitude, ☉, in radians
  {Number} ano - true anomaly in radians  

| Param | Type | Description |
| --- | --- | --- |
| T | <code>Number</code> | number of Julian centuries since J2000. See base.J2000Century. |

<a name="module_solar.trueEquatorial"></a>

### solar.trueEquatorial(jde) ⇒ <code>base.Coord</code>
trueEquatorial returns the true geometric position of the Sun as equatorial coordinates.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>base.Coord</code> - {Number} ra - right ascension in radians
  {Number} dec - declination in radians  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solar.apparentEquatorial"></a>

### solar.apparentEquatorial(jde) ⇒ <code>base.Coord</code>
apparentEquatorial returns the apparent position of the Sun as equatorial coordinates.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>base.Coord</code> - {Number} ra - right ascension in radians
  {Number} dec - declination in radians  

| Param | Type | Description |
| --- | --- | --- |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solar.trueVSOP87"></a>

### solar.trueVSOP87(planet, jde) ⇒ <code>Object</code>
trueVSOP87 returns the true geometric position of the sun as ecliptic coordinates.

Result computed by full VSOP87 theory.  Result is at equator and equinox
of date in the FK5 frame.  It does not include nutation or aberration.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Object</code> - {Number} lon - ecliptic longitude in radians
  {Number} lat - ecliptic latitude in radians
  {Number} range - range in AU  

| Param | Type | Description |
| --- | --- | --- |
| planet | <code>planetposition.Planet</code> |  |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solar.apparentVSOP87"></a>

### solar.apparentVSOP87(planet, jde) ⇒ <code>base.Coord</code>
apparentVSOP87 returns the apparent position of the sun as ecliptic coordinates.

Result computed by VSOP87, at equator and equinox of date in the FK5 frame,
and includes effects of nutation and aberration.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>base.Coord</code> - {Number} lon - ecliptic longitude in radians
  {Number} lat - ecliptic latitude in radians
  {Number} range - range in AU  

| Param | Type | Description |
| --- | --- | --- |
| planet | <code>planetposition.Planet</code> |  |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solar.apparentEquatorialVSOP87"></a>

### solar.apparentEquatorialVSOP87(planet, jde) ⇒ <code>Number</code>
apparentEquatorialVSOP87 returns the apparent position of the sun as equatorial coordinates.

Result computed by VSOP87, at equator and equinox of date in the FK5 frame,
and includes effects of nutation and aberration.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - ra - right ascension in radians
  {Number} dec - declination in radians
  {Number} range - range in AU  

| Param | Type | Description |
| --- | --- | --- |
| planet | <code>planetposition.Planet</code> |  |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solar.aberration"></a>

### solar.aberration(range) ⇒ <code>Number</code>
Low precision formula.  The high precision formula is not implemented
because the low precision formula already gives position results to the
accuracy given on p. 165.  The high precision formula represents lots
of typing with associated chance of typos, and no way to test the result.

**Kind**: static method of [<code>solar</code>](#module_solar)  
**Returns**: <code>Number</code> - aberation  

| Param | Type |
| --- | --- |
| range | <code>Number</code> | 

<a name="module_solardisk"></a>

## solardisk
**License**: MIT  
**Copyright**: 2016 commenthol  

* [solardisk](#module_solardisk)
    * [.ephemeris()](#module_solardisk.ephemeris)
    * [.cycle()](#module_solardisk.cycle)

<a name="module_solardisk.ephemeris"></a>

### solardisk.ephemeris()
Ephemeris returns the apparent orientation of the sun at the given jd.

Results:
 P:  Position angle of the solar north pole.
 B0: Heliographic latitude of the center of the solar disk.
 L0: Heliographic longitude of the center of the solar disk.

All results in radians.

**Kind**: static method of [<code>solardisk</code>](#module_solardisk)  
<a name="module_solardisk.cycle"></a>

### solardisk.cycle()
Cycle returns the jd of the start of the given synodic rotation.

Argument c is the "Carrington" cycle number.

Result is a dynamical time (not UT).

**Kind**: static method of [<code>solardisk</code>](#module_solardisk)  
<a name="module_solarxyz"></a>

## solarxyz
**License**: MIT  
**Copyright**: 2016 commenthol  

* [solarxyz](#module_solarxyz)
    * [.position(earth, jde)](#module_solarxyz.position) ⇒ <code>object</code>
    * [.longitudeJ2000(earth, jde)](#module_solarxyz.longitudeJ2000) ⇒ <code>Number</code>
    * [.positionJ2000(earth, jde)](#module_solarxyz.positionJ2000) ⇒ <code>object</code>
    * [.positionB1950(earth, jde)](#module_solarxyz.positionB1950) ⇒ <code>object</code>
    * [.positionEquinox(earth, jde, epoch)](#module_solarxyz.positionEquinox) ⇒ <code>object</code>

<a name="module_solarxyz.position"></a>

### solarxyz.position(earth, jde) ⇒ <code>object</code>
Position returns rectangular coordinates referenced to the mean equinox of date.

**Kind**: static method of [<code>solarxyz</code>](#module_solarxyz)  
**Returns**: <code>object</code> - rectangular coordinates
  {Number} x
  {Number} y
  {Number} z  

| Param | Type | Description |
| --- | --- | --- |
| earth | <code>planetposition.Planet</code> | VSOP87Planet Earth |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solarxyz.longitudeJ2000"></a>

### solarxyz.longitudeJ2000(earth, jde) ⇒ <code>Number</code>
LongitudeJ2000 returns geometric longitude referenced to equinox J2000.

**Kind**: static method of [<code>solarxyz</code>](#module_solarxyz)  
**Returns**: <code>Number</code> - geometric longitude referenced to equinox J2000.  

| Param | Type | Description |
| --- | --- | --- |
| earth | <code>planetposition.Planet</code> | VSOP87Planet Earth |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solarxyz.positionJ2000"></a>

### solarxyz.positionJ2000(earth, jde) ⇒ <code>object</code>
PositionJ2000 returns rectangular coordinates referenced to equinox J2000.

**Kind**: static method of [<code>solarxyz</code>](#module_solarxyz)  
**Returns**: <code>object</code> - rectangular coordinates
  {Number} x
  {Number} y
  {Number} z  

| Param | Type | Description |
| --- | --- | --- |
| earth | <code>planetposition.Planet</code> | VSOP87Planet Earth |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solarxyz.positionB1950"></a>

### solarxyz.positionB1950(earth, jde) ⇒ <code>object</code>
PositionB1950 returns rectangular coordinates referenced to B1950.

Results are referenced to the mean equator and equinox of the epoch B1950
in the FK5 system, not FK4.

**Kind**: static method of [<code>solarxyz</code>](#module_solarxyz)  
**Returns**: <code>object</code> - rectangular coordinates
  {Number} x
  {Number} y
  {Number} z  

| Param | Type | Description |
| --- | --- | --- |
| earth | <code>planetposition.Planet</code> | VSOP87Planet Earth |
| jde | <code>Number</code> | Julian ephemeris day |

<a name="module_solarxyz.positionEquinox"></a>

### solarxyz.positionEquinox(earth, jde, epoch) ⇒ <code>object</code>
PositionEquinox returns rectangular coordinates referenced to an arbitrary epoch.

Position will be computed for given Julian day "jde" but referenced to mean
equinox "epoch" (year).

**Kind**: static method of [<code>solarxyz</code>](#module_solarxyz)  
**Returns**: <code>object</code> - rectangular coordinates
  {Number} x
  {Number} y
  {Number} z  

| Param | Type | Description |
| --- | --- | --- |
| earth | <code>planetposition.Planet</code> | VSOP87Planet Earth |
| jde | <code>Number</code> | Julian ephemeris day |
| epoch | <code>Number</code> |  |

<a name="module_solstice"></a>

## solstice
**License**: MIT  
**Copyright**: 2016 commenthol  

* [solstice](#module_solstice)
    * _static_
        * [.march(y)](#module_solstice.march) ⇒ <code>Number</code>
        * [.june(y)](#module_solstice.june) ⇒ <code>Number</code>
        * [.september(y)](#module_solstice.september) ⇒ <code>Number</code>
        * [.december(y)](#module_solstice.december) ⇒ <code>Number</code>
        * [.march2(year, planet)](#module_solstice.march2) ⇒ <code>Number</code>
        * [.june2(year, planet)](#module_solstice.june2) ⇒ <code>Number</code>
        * [.september2(year, planet)](#module_solstice.september2) ⇒ <code>Number</code>
        * [.december2(year, planet)](#module_solstice.december2) ⇒ <code>Number</code>
        * [.longitude(year, planet, lon)](#module_solstice.longitude) ⇒ <code>Number</code>
    * _inner_
        * [~eq(y, c)](#module_solstice..eq) ⇒ <code>Number</code>
        * [~eq2(year, planet, lon, c)](#module_solstice..eq2) ⇒ <code>Number</code>

<a name="module_solstice.march"></a>

### solstice.march(y) ⇒ <code>Number</code>
March returns the JDE of the March equinox for the given year.

Results are valid for the years -1000 to +3000.

Accuracy is within one minute of time for the years 1951-2050.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | (int) year |

<a name="module_solstice.june"></a>

### solstice.june(y) ⇒ <code>Number</code>
June returns the JDE of the June solstice for the given year.

Results are valid for the years -1000 to +3000.

Accuracy is within one minute of time for the years 1951-2050.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | (int) year |

<a name="module_solstice.september"></a>

### solstice.september(y) ⇒ <code>Number</code>
September returns the JDE of the September equinox for the given year.

Results are valid for the years -1000 to +3000.

Accuracy is within one minute of time for the years 1951-2050.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | (int) year |

<a name="module_solstice.december"></a>

### solstice.december(y) ⇒ <code>Number</code>
December returns the JDE of the December solstice for a given year.

Results are valid for the years -1000 to +3000.

Accuracy is within one minute of time for the years 1951-2050.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | (int) year |

<a name="module_solstice.march2"></a>

### solstice.march2(year, planet) ⇒ <code>Number</code>
March2 returns a more accurate JDE of the March equinox.

Result is accurate to one second of time.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) year |
| planet | <code>planetposition.Planet</code> | must be a V87Planet object representing Earth, obtained with the package planetposition |

<a name="module_solstice.june2"></a>

### solstice.june2(year, planet) ⇒ <code>Number</code>
June2 returns a more accurate JDE of the June solstice.

Result is accurate to one second of time.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) year |
| planet | <code>planetposition.Planet</code> | must be a V87Planet object representing Earth, obtained with the package planetposition |

<a name="module_solstice.september2"></a>

### solstice.september2(year, planet) ⇒ <code>Number</code>
September2 returns a more accurate JDE of the September equinox.

Result is accurate to one second of time.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) year |
| planet | <code>planetposition.Planet</code> | must be a V87Planet object representing Earth, obtained with the package planetposition |

<a name="module_solstice.december2"></a>

### solstice.december2(year, planet) ⇒ <code>Number</code>
December2 returns a more accurate JDE of the December solstice.

Result is accurate to one second of time.

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) year |
| planet | <code>planetposition.Planet</code> | must be a V87Planet object representing Earth, obtained with the package planetposition |

<a name="module_solstice.longitude"></a>

### solstice.longitude(year, planet, lon) ⇒ <code>Number</code>
Longitude returns the JDE for a given `year`, VSOP87 Planet `planet` at a
given geocentric solar longitude `lon`

**Kind**: static method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) |
| planet | <code>planetposition.Planet</code> |  |
| lon | <code>Number</code> | geocentric solar longitude in radians |

<a name="module_solstice..eq"></a>

### solstice~eq(y, c) ⇒ <code>Number</code>
Fast calculation of solstices/ equinoxes
Accuracy is within one minute of time for the years 1951-2050.

**Kind**: inner method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| y | <code>Number</code> | (int) year |
| c | <code>Array</code> | term from table 27.a / 27.b |

<a name="module_solstice..eq2"></a>

### solstice~eq2(year, planet, lon, c) ⇒ <code>Number</code>
Accurate calculation of solstices/ equinoxes
Result is accurate to one second of time.

**Kind**: inner method of [<code>solstice</code>](#module_solstice)  
**Returns**: <code>Number</code> - JDE  

| Param | Type | Description |
| --- | --- | --- |
| year | <code>Number</code> | (int) year |
| planet | <code>planetposition.Planet</code> | vsop87 planet |
| lon | <code>Number</code> | longitude in radians |
| c | <code>Array</code> | term from table 27.a / 27.b |

<a name="module_stellar"></a>

## stellar
**License**: MIT  
**Copyright**: 2016 commenthol  

* [stellar](#module_stellar)
    * [.sum()](#module_stellar.sum)
    * [.sumN()](#module_stellar.sumN)
    * [.ratio()](#module_stellar.ratio)
    * [.difference()](#module_stellar.difference)
    * [.absoluteByParallax()](#module_stellar.absoluteByParallax)
    * [.absoluteByDistance()](#module_stellar.absoluteByDistance)

<a name="module_stellar.sum"></a>

### stellar.sum()
Sum returns the combined apparent magnitude of two stars.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_stellar.sumN"></a>

### stellar.sumN()
SumN returns the combined apparent magnitude of a number of stars.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_stellar.ratio"></a>

### stellar.ratio()
Ratio returns the brightness ratio of two stars.

Arguments m1, m2 are apparent magnitudes.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_stellar.difference"></a>

### stellar.difference()
Difference returns the difference in apparent magnitude of two stars
given their brightness ratio.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_stellar.absoluteByParallax"></a>

### stellar.absoluteByParallax()
AbsoluteByParallax returns absolute magnitude given annual parallax.

Argument m is apparent magnitude, π is annual parallax in arc seconds.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_stellar.absoluteByDistance"></a>

### stellar.absoluteByDistance()
AbsoluteByDistance returns absolute magnitude given distance.

Argument m is apparent magnitude, d is distance in parsecs.

**Kind**: static method of [<code>stellar</code>](#module_stellar)  
<a name="module_sundial"></a>

## sundial
**License**: MIT  
**Copyright**: 2016 commenthol  

* [sundial](#module_sundial)
    * _static_
        * [.general()](#module_sundial.general)
        * [.equatorial()](#module_sundial.equatorial)
        * [.horizontal()](#module_sundial.horizontal)
        * [.vertical()](#module_sundial.vertical)
    * _inner_
        * [~Point()](#module_sundial..Point)
        * [~Line()](#module_sundial..Line)

<a name="module_sundial.general"></a>

### sundial.general()
General computes data for the general case of a planar sundial.

Argument φ is geographic latitude at which the sundial will be located.
D is gnomonic declination, the azimuth of the perpendicular to the plane
of the sundial, measured from the southern meridian towards the west.
Argument a is the length of a straight stylus perpendicular to the plane
of the sundial, z is zenithal distance of the direction defined by the
stylus.  Angles φ, D, and z are in radians.  Units of stylus length a
are arbitrary.

Results consist of a set of lines, a center point, u, the length of a
polar stylus, and ψ, the angle which the polar stylus makes with the plane
of the sundial.  The center point, the points defining the hour lines, and
u are in units of a, the stylus length.  ψ is in radians.

**Kind**: static method of [<code>sundial</code>](#module_sundial)  
<a name="module_sundial.equatorial"></a>

### sundial.equatorial()
Equatorial computes data for a sundial level with the equator.

Argument φ is geographic latitude at which the sundial will be located;
a is the length of a straight stylus perpendicular to the plane of the
sundial.

The sundial will have two sides, north and south.  Results n and s define
lines on the north and south sides of the sundial.  Result coordinates
are in units of a, the stylus length.

**Kind**: static method of [<code>sundial</code>](#module_sundial)  
<a name="module_sundial.horizontal"></a>

### sundial.horizontal()
Horizontal computes data for a horizontal sundial.

Argument φ is geographic latitude at which the sundial will be located,
a is the length of a straight stylus perpendicular to the plane of the
sundial.

Results consist of a set of lines, a center point, and u, the length of a
polar stylus.  They are in units of a, the stylus length.

**Kind**: static method of [<code>sundial</code>](#module_sundial)  
<a name="module_sundial.vertical"></a>

### sundial.vertical()
Vertical computes data for a vertical sundial.

Argument φ is geographic latitude at which the sundial will be located.
D is gnomonic declination, the azimuth of the perpendicular to the plane
of the sundial, measured from the southern meridian towards the west.
Argument a is the length of a straight stylus perpendicular to the plane
of the sundial.

Results consist of a set of lines, a center point, and u, the length of a
polar stylus.  They are in units of a, the stylus length.

**Kind**: static method of [<code>sundial</code>](#module_sundial)  
<a name="module_sundial..Point"></a>

### sundial~Point()
Point return type represents a point to be used in constructing the sundial.

**Kind**: inner method of [<code>sundial</code>](#module_sundial)  
<a name="module_sundial..Line"></a>

### sundial~Line()
Line holds data to draw an hour line on the sundial.

**Kind**: inner method of [<code>sundial</code>](#module_sundial)  
<a name="module_sunrise"></a>

## sunrise
**License**: MIT  
**Copyright**: 2016 commenthol  

* [sunrise](#module_sunrise)
    * [.Sunrise](#module_sunrise.Sunrise)
        * [new exports.Sunrise(date, lat, lon, [refraction])](#new_module_sunrise.Sunrise_new)
        * [.noon()](#module_sunrise.Sunrise+noon) ⇒ <code>julian.Calendar</code>
        * [.rise()](#module_sunrise.Sunrise+rise) ⇒ <code>julian.Calendar</code>
        * [.set()](#module_sunrise.Sunrise+set) ⇒ <code>julian.Calendar</code>
        * [.riseEnd()](#module_sunrise.Sunrise+riseEnd) ⇒ <code>julian.Calendar</code>
        * [.setStart()](#module_sunrise.Sunrise+setStart) ⇒ <code>julian.Calendar</code>
        * [.dawn()](#module_sunrise.Sunrise+dawn) ⇒ <code>julian.Calendar</code>
        * [.dusk()](#module_sunrise.Sunrise+dusk) ⇒ <code>julian.Calendar</code>
        * [.nauticalDawn()](#module_sunrise.Sunrise+nauticalDawn) ⇒ <code>julian.Calendar</code>
        * [.nauticalDusk()](#module_sunrise.Sunrise+nauticalDusk) ⇒ <code>julian.Calendar</code>
        * [.nightStart()](#module_sunrise.Sunrise+nightStart) ⇒ <code>julian.Calendar</code>
        * [.nightEnd()](#module_sunrise.Sunrise+nightEnd) ⇒ <code>julian.Calendar</code>
        * [.goldenHourStart()](#module_sunrise.Sunrise+goldenHourStart) ⇒ <code>julian.Calendar</code>
        * [.goldenHourEnd()](#module_sunrise.Sunrise+goldenHourEnd) ⇒ <code>julian.Calendar</code>

<a name="module_sunrise.Sunrise"></a>

### sunrise.Sunrise
**Kind**: static class of [<code>sunrise</code>](#module_sunrise)  

* [.Sunrise](#module_sunrise.Sunrise)
    * [new exports.Sunrise(date, lat, lon, [refraction])](#new_module_sunrise.Sunrise_new)
    * [.noon()](#module_sunrise.Sunrise+noon) ⇒ <code>julian.Calendar</code>
    * [.rise()](#module_sunrise.Sunrise+rise) ⇒ <code>julian.Calendar</code>
    * [.set()](#module_sunrise.Sunrise+set) ⇒ <code>julian.Calendar</code>
    * [.riseEnd()](#module_sunrise.Sunrise+riseEnd) ⇒ <code>julian.Calendar</code>
    * [.setStart()](#module_sunrise.Sunrise+setStart) ⇒ <code>julian.Calendar</code>
    * [.dawn()](#module_sunrise.Sunrise+dawn) ⇒ <code>julian.Calendar</code>
    * [.dusk()](#module_sunrise.Sunrise+dusk) ⇒ <code>julian.Calendar</code>
    * [.nauticalDawn()](#module_sunrise.Sunrise+nauticalDawn) ⇒ <code>julian.Calendar</code>
    * [.nauticalDusk()](#module_sunrise.Sunrise+nauticalDusk) ⇒ <code>julian.Calendar</code>
    * [.nightStart()](#module_sunrise.Sunrise+nightStart) ⇒ <code>julian.Calendar</code>
    * [.nightEnd()](#module_sunrise.Sunrise+nightEnd) ⇒ <code>julian.Calendar</code>
    * [.goldenHourStart()](#module_sunrise.Sunrise+goldenHourStart) ⇒ <code>julian.Calendar</code>
    * [.goldenHourEnd()](#module_sunrise.Sunrise+goldenHourEnd) ⇒ <code>julian.Calendar</code>

<a name="new_module_sunrise.Sunrise_new"></a>

#### new exports.Sunrise(date, lat, lon, [refraction])
Computes time of sunrise, sunset for a given day `date` of an observer on earth given by latitude and longitude.
Methods may return `undefined` instead of `julian.Calendar` for latitudes very near the poles.


| Param | Type | Description |
| --- | --- | --- |
| date | <code>julian.Calendar</code> | calendar date |
| lat | <code>number</code> | latitude of observer in the range of (-89.6, 89.6) |
| lon | <code>number</code> | longitude of observer (measured positively westwards, New York = 40.7° lat, 74° lon) |
| [refraction] | <code>number</code> | optional refraction |

<a name="module_sunrise.Sunrise+noon"></a>

#### sunrise.noon() ⇒ <code>julian.Calendar</code>
time of solar transit

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of noon  
<a name="module_sunrise.Sunrise+rise"></a>

#### sunrise.rise() ⇒ <code>julian.Calendar</code>
Solar limb appears over the easter horizon in the morning

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of sunrise  
<a name="module_sunrise.Sunrise+set"></a>

#### sunrise.set() ⇒ <code>julian.Calendar</code>
**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of sunset
Solar limb disappears on the western horizon in the evening  
<a name="module_sunrise.Sunrise+riseEnd"></a>

#### sunrise.riseEnd() ⇒ <code>julian.Calendar</code>
Solar limb is fully visible at the easter horizon

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of sunrise end  
<a name="module_sunrise.Sunrise+setStart"></a>

#### sunrise.setStart() ⇒ <code>julian.Calendar</code>
Solar limb starts disappearing on the western horizon in the evening

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of sunset start  
<a name="module_sunrise.Sunrise+dawn"></a>

#### sunrise.dawn() ⇒ <code>julian.Calendar</code>
Dawn, there is still enough light for objects to be distinguishable,

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of dawn  
<a name="module_sunrise.Sunrise+dusk"></a>

#### sunrise.dusk() ⇒ <code>julian.Calendar</code>
Dusk, there is still enough light for objects to be distinguishable
Bright stars and planets are visible by naked eye

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of dusk  
<a name="module_sunrise.Sunrise+nauticalDawn"></a>

#### sunrise.nauticalDawn() ⇒ <code>julian.Calendar</code>
nautical dawn - Horizon gets visible by naked eye

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of nautical dawn  
<a name="module_sunrise.Sunrise+nauticalDusk"></a>

#### sunrise.nauticalDusk() ⇒ <code>julian.Calendar</code>
nautical dusk - Horizon is no longer visible by naked eye

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of nautical dusk  
<a name="module_sunrise.Sunrise+nightStart"></a>

#### sunrise.nightStart() ⇒ <code>julian.Calendar</code>
night starts - No sunlight illumination of the sky, such no intereferance
with astronomical observations.

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of start of night  
<a name="module_sunrise.Sunrise+nightEnd"></a>

#### sunrise.nightEnd() ⇒ <code>julian.Calendar</code>
night end - Sunlight starts illumination of the sky and interferes
with astronomical observations.

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of end of night  
<a name="module_sunrise.Sunrise+goldenHourStart"></a>

#### sunrise.goldenHourStart() ⇒ <code>julian.Calendar</code>
Start of "golden hour" before sunset

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of start of golden hour  
<a name="module_sunrise.Sunrise+goldenHourEnd"></a>

#### sunrise.goldenHourEnd() ⇒ <code>julian.Calendar</code>
End of "golden hour" after sunrise

**Kind**: instance method of [<code>Sunrise</code>](#module_sunrise.Sunrise)  
**Returns**: <code>julian.Calendar</code> - time of end of golden hour  
<a name="module_vsop87"></a>

## vsop87
**License**: MIT  
**Copyright**: 2016 commenthol  

* [vsop87](#module_vsop87)
    * [.VSOP](#module_vsop87.VSOP)
        * [new exports.VSOP(planet, dirname, [opts])](#new_module_vsop87.VSOP_new)
        * [._getExt()](#module_vsop87.VSOP+_getExt)
        * [.load()](#module_vsop87.VSOP+load)
        * [.loadSync()](#module_vsop87.VSOP+loadSync)
        * [.parse(data)](#module_vsop87.VSOP+parse)
        * [.getData()](#module_vsop87.VSOP+getData) ⇒ <code>Object</code>

<a name="module_vsop87.VSOP"></a>

### vsop87.VSOP
**Kind**: static class of [<code>vsop87</code>](#module_vsop87)  

* [.VSOP](#module_vsop87.VSOP)
    * [new exports.VSOP(planet, dirname, [opts])](#new_module_vsop87.VSOP_new)
    * [._getExt()](#module_vsop87.VSOP+_getExt)
    * [.load()](#module_vsop87.VSOP+load)
    * [.loadSync()](#module_vsop87.VSOP+loadSync)
    * [.parse(data)](#module_vsop87.VSOP+parse)
    * [.getData()](#module_vsop87.VSOP+getData) ⇒ <code>Object</code>

<a name="new_module_vsop87.VSOP_new"></a>

#### new exports.VSOP(planet, dirname, [opts])
load VSOP87 planet data from VSOP87 files
Data can be obtained from ftp://cdsarc.u-strasbg.fr/pub/cats/VI%2F81/

**Throws**:

- <code>Error</code> 


| Param | Type | Description |
| --- | --- | --- |
| planet | <code>String</code> | MERCURY VENUS EARTH MARS JUPITER SATURN URANUS NEPTUNE |
| dirname | <code>String</code> | folder containing VSOP87 files |
| [opts] | <code>Object</code> |  |
| [opts.type] | <code>String</code> | file type A, B, C, D - See vsop87.txt |

<a name="module_vsop87.VSOP+_getExt"></a>

#### vsoP.\_getExt()
get file extension for planet

**Kind**: instance method of [<code>VSOP</code>](#module_vsop87.VSOP)  
<a name="module_vsop87.VSOP+load"></a>

#### vsoP.load()
load data from file

**Kind**: instance method of [<code>VSOP</code>](#module_vsop87.VSOP)  
<a name="module_vsop87.VSOP+loadSync"></a>

#### vsoP.loadSync()
sync loading

**Kind**: instance method of [<code>VSOP</code>](#module_vsop87.VSOP)  
<a name="module_vsop87.VSOP+parse"></a>

#### vsoP.parse(data)
parse data

**Kind**: instance method of [<code>VSOP</code>](#module_vsop87.VSOP)  

| Param | Type | Description |
| --- | --- | --- |
| data | <code>String</code> | content of VSOP file |

<a name="module_vsop87.VSOP+getData"></a>

#### vsoP.getData() ⇒ <code>Object</code>
get parsed data

**Kind**: instance method of [<code>VSOP</code>](#module_vsop87.VSOP)  
**Returns**: <code>Object</code> - { L: { '0': [[A, B, C], ...], '1': [], '2': [], '3': [], '4': [], '5': [] },
  B: { '0': [], '1': [], '2': [], '3': [], '4': [], '5': [] },
  R: { '0': [], '1': [], '2': [], '3': [], '4': [], '5': [] } }  
<a name="Planet"></a>

## Planet
**Kind**: global class  
<a name="new_Planet_new"></a>

### new exports.Planet(planet)
VSOP87 representation of a Planet


| Param | Type | Description |
| --- | --- | --- |
| planet | <code>object</code> | planet data series |

**Example**  
```js
// for use in browser
import {data} from 'astronomia.js'
const earth = new planetposition.Planet(data.vsop87Bearth)
```
